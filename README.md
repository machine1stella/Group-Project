# Group-Project
## Files:
- original_code-Copy1.ipynb (Code me found on salesman tabu search problem)
- tabu.py (did some change on the previous origianl file, and save the origin code as py.file )
- Multiprocess.ipynb (to do the parallel, me need to import the tabu.py above.)

## Steps:
- 1. Open tabu.py, set the parameters(iteration numbers, tabu list size and size)
- 2. Open the Multiprocess.ipynb. Build a new `city_list` contain 30 different routes(different from the start and end cities.)
- 3. Do the parallel by using the Multiprocess package. 
- 4. Parallel the `tabu.parallelfunc` with `city_list`
- 5. It returns a list which contain 30 optimal answers (best answer for each routes)
- 6. At end, `finalanswer` helps find the best amoung these 30 answers. and return the star-end city number, the travel distacne and route.

## Details:
- Open original_code-Copy1.ipynb
- `printtravel(vec)` returns the route. For example, the set the start city and end city to be **1**, the initial route is 1-2-3-,....28-29-30-1.
- `costroad` returns the travel distance of the route.
- `tabusearch(diedaitimes,cacu_time,tabu_length,origin_times,costf,printf)` returns the excuted time, the best travel distance and route.
- If the trip started from city3 then it will ended in city3. `tabusearch` function can only apply on one city.
- In tabu.py, I added `parallelfunc(aa)` function. the input aa is the city number. 

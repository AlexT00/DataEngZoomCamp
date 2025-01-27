Codes used for homework:
# Question 1
docker run -it python:3.12.8 bash
pip -V
Answer: 24.3.1

# Question 2
Hostname: db
Port: 5432

# Question 3
SELECT count(1) from green_taxi_data WHERE trip_distance <= 1
SELECT count(1) from green_taxi_data WHERE trip_distance > 1 and trip_distance <= 3
SELECT count(1) from green_taxi_data WHERE trip_distance > 3 and trip_distance <= 7
SELECT count(1) from green_taxi_data WHERE trip_distance > 7 and trip_distance <= 10
SELECT count(1) from green_taxi_data WHERE trip_distance > 10

Ans: 104,838; 199,013; 109,645; 27,688; 35,202
# Question 4
SELECT lpep_pickup_datetime, trip_distance FROM green_taxi_data ORDER BY trip_distance DESC LIMIT 1;

Ans: 2019-10-31

# Question 5

SELECT "PULocationID", SUM(total_amount) as amount FROM green_taxi_data WHERE DATE(lpep_pickup_datetime) = '2019-10-18' GROUP BY "PULocationID" HAVING SUM(total_amount) > 13000 ORDER BY amount DESC LIMIT 3;

ANS:  74, 75, 166
East Harlem North
East Harlem South
Morningside Heights

# Question 6

SELECT "DOLocationID", tip_amount FROM green_taxi_data WHERE "PULocationID" = 74 ORDER BY tip_amount DESC LIMIT 1
Ans: 132, JFK Airport

# Question 7
Ans: terraform init, terraform apply -auto-approve, terraform destroy


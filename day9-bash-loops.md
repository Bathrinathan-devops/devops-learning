### DAY 9 loops in bash

##Loop 1 - FOR loop:

for i in {1..5}
do
echo "number $i"
done
use : when you know exact repetitions

************************

##Loop 2 - WHILE loop:
COUNT=1
while [ $COUNT -le 5 ]
do
echo "count is $COUNT"
COUNT=$((COUNT + 1 ))
done
use: repeat while condition is TURE , stops when condition becoms false
*******************

##LOOP 3 - UNTIL Loop:
COUNT=1
until [ $COUNT -gt 5 ]
do
echo "count is $COUNT"
COUNT=$((COUNT + 1 ))
done
use : repeat until condtion becoms TRUE, STOPS when conditions becoms true

#### Mandatory words

for - do - done

while - do - done

until - do - done
##KEY different
for - fixed number of times
while- run when green  light
until- run when red light 

###Imnportant rule:
Always increment counter in while/until 
COUNT=$(($COUNT + 1 ))
without this infinte loop forevrer

#Day9 - IF condition in bash

### Form 1- Simple IF:
if [ condition ]
then
 echo "do something"
fi
*********************
Form 2 - IF ELSE:

if [ condition ]
then
echo "true"
else
echo "false"
fi

**********************

FORM 3 - IF ELIF ELSE:

if [ condition1 ]
then
   echo "first"
elif [ condition 2 ]
then
  echo " second"

  else
     echo "neither"

    fi

    *************************
##### Comparision operators;
-eq  __ eual ti
-ne __ not equal to
-gt __greater then 
-lt __less than
-le ++less than ir qual to
-ge __greathen than or qual to 

######## Special opeaators:

% - remainder (Modulo)
- even: $((I % 2 )) -eq 0
- odd: $((I % 2 )) -ne 0

  ###Mandtory words:
  if - then - fi
  

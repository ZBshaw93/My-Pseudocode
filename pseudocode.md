My Pseudocode

Functionality

Main Goal- 

The user should be able to know the proper basketball size, basketball weight, basketball goal size, and free throw length in order to shoot a proper free throw. 

Things to keep in mind-

- If the basketball is too big or too small it will affect the proper free throw.

- If the basketball has too much or not enough air it will affect the proper free throw.

- If the basketball goal is too far or too short from the user it will affect the proper free throw.

- If the basketball goal is too tall or too short it will affect the proper free throw.

Objects-

- Basketball - 29.5 inches long
- Pump- 7.5-8.5 psi
- Basketball goal - 10 feet high
- Basketball free throw line approximately  15 feet away from the basket.
- Measuring tape - Measure free throw distance, ball size and goal height.

Pseudocode

1. Define objects and functions.

- Basketball

* basketballSmall —> currentBall ++
* basketballBig —> currentBall - -
* basketballGood —> currentBall === goodBall
* shootHarder —> currentShot++
* shootSofter —> currentShot- -
* shootSame —> currentShot === madeShot
* currentShot —> Last taken shot from user.
* INIT basketballSizeGood()

- Measuring Tape

* INIT readTape() —> Measuring tape shows measurement.
* INIT userCall() —> Tells user if measurement is too long or too short.
* INIT userMeasurement() —> Tells user the correct measurement to use.

- Basketball pump

* pumpMore —> currentAir++
* pumpLess —> currentAir- -
* pumpGood —> currentAir === goodAir

- Basketball Goal

* goalShort —> currentGoal++
* goalTall—> currentGoal- -
* goalGood —> currentGoal === goodGoal

- Basketball free throw line

* lineShort —> currentLine++
* lineLong —> currentLine- -
* lineGood —> currentLine === goodLine
* shootFreeThrow() —> User ready to shoot free throw.

2. Brief Overview Example

START

// Function to establish correct measurements of a good size ball //

IF currentBall != goodBall
    THEN
             WHILE currentBall > goodBall
                    basketballBig
                    break
             WHILE currentBall < goodBall
                    basketballSmall
                    break
             END WHILE
ELSE shootFreeThow()


// Function to establish correct measurements from user to basketball goal //

IF currentLine != lineGood
    THEN
          WHILE currentLine > lineGood
                 lineLong
                 break
           WHILE currentLine < lineGood
                 lineShort
                 break
            END WHILE
ELSE shootFreeThrow()


// Function to establish correct height of the basketball goal //

IF currentGoal != goalGood
    THEN
          WHILE currentGoal > goalGood
                 lineTall
                 break
           WHILE currentGoal < goalGood
                 lineShort
                 break
            END WHILE
ELSE shootFreeThrow()

// Function to establish correct air pressure of a basketball //

IF currentAir != pumpGood
    THEN
          WHILE currentAir > pumpGood
                 pumpLess
                 break
           WHILE currentAir < pumpGood
                 pumpMore
                 break
            END WHILE
ELSE shootFreeThrow()

END
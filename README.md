// Each letter represents a unique digit (0–9)
CREATE empty mapping LetterToDigit
CREATE set of all unique letters

IF number of unique letters > 10 THEN
    PRINT "No solution"
    STOP
END IF

ASSIGN digits 0–9 to letters using permutation

FOR each assignment DO
    IF any leading letter has digit 0 THEN
        CONTINUE
    END IF

    CONVERT each word into number using assignment

    IF sum of word numbers = result number THEN
        PRINT "Solution found"
        PRINT assignment
        STOP
    END IF
END FOR

PRINT "No solution exists"

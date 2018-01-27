# D20-Roller
A d20 die roller / random number generator
FUNCTION initialize()
myWin = newWindow("D20 ROLLER", 500, 500)
my TextBox = newTextBox(myWin,"…", 140, 200, 220, 60)
rollButton = newButton.addClickHandler(rollD20)
END
FUNCTION rollD20()
randNum = randomInteger(1,20)
myTextBox.text = toString(randNum)
IF randNum <20 THEN
	myWin.bgColor = Color.white
ELSE
	myWin.bgColor = Color.green
ENDIF
END

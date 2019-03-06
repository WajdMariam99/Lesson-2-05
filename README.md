# Lesson-2-05
-----------------------------------------------------------------------------------------
--
-- how to add a text field and button, so that you can enter text
--

-----------------------------------------------------------------------------------------
--
-- how to add a text field and button, so that you can enter text
--
-----------------------------------------------------------------------------------------

local answerTextField = native.newTextField( display.contentCenterX, display.contentCenterY + 200, 450, 75 )
answerTextField.id = "answer textField"

local enterButton = display.newImageRect( "./Assests/sprites/enterButton", 406, 157 )
enterButton.x = 375
enterButton.y = 500
enterButton.id = "enter button"
 
local function enterButtonTouch( event )
    -- it is not perfect, but we will make it better soon
    print( answerTextField.text )
   
    return true
end

enterButton:addEventListener( "touch", enterButtonTouch)

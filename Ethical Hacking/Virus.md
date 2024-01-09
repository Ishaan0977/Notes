
### Turn off internet connection
@Echo off
Ipconfig /release
### Turn on internet connection
@Echo off
Ipconfig /renew

### Pop up window

X=MsgBox("Your text here",num1 + num2 , "Tittle")

num 1 is for type of buttons in pop up 
- 0 = OK
- 1= Ok and cancel
- 2= Abort , retry and ignore button
- 3= Yes,No and cancel
- 4=Yes and NO
- 5= Retry and cancel
Num 2 is for type of icons 
- 16 = critical icon
- 32 = Help Icon
- 48 = Warning icon
- 64 = Information icon

### Trojan
- ProRat can be used to create trojan

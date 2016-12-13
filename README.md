@echo off
cls
echo Hello and welcome.
:loop
:menu
cls
color 0a
color 1a
cls 
echo 1.)start
echo 2.)exit
set /p number=

if %number% == 1 goto game
if %number% == 2 Exit


if not defined number (
cls
goto loop
) 

:Game
cls
echo Hello whats your name???
set /p name=
cls 
hello %name% would you like to start the game???(y/n)
set /p hey=

if %hey% == y goto youwin 
if %hey% == n menu
if %hey% == N menu
if %hey% == Y goto youwin



:you Win
cls 
echo wow that was hard how did you win???
echo by 
goto menu 

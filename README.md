# gotcha
Thanks for indulging me! This simple script is a mini Frankenstein's Monster made of a couple things I found online and thought would be more usefull together. When an incorrect password is entered, either in the terminal or the initial graphical login, the script interfaces with the webcam, takes a picture, and sends the picture to a designated email.
This is accomplished by sticking a well known script and the sendEmail program together. Basically, I'm just steling everyones stuff and calling it "neat".

Start by uncompressing the file folder into your Downloads directory. Then open a terminal, type "cd Downloads/gotcha", make the install script executable by typing "chmod +x install" and then type "./install". The rest should be taken care of for you, becaus I know how much laziness can stop us from doing simple things. 

After it's all installed you'll just have to change a few things in the script file in /usr/local/bin/gotcha.
In the variables section at the top, just change the following to match your settings and email prefferences, leaving out the quotation marks (with the exception of the SUBJECT and MESSAGE lines):

SMTPFROM="from email@address.com"
SMTPTO="to email@address.com"
SMTPSERVER="your email service address followed by the email smtp number, example:smtp.googlemail.com:587"
SMTPUSER="your SMTPFROM username here, example: eamil@address.com"
SMTPPASS="your smtp password here"
SUBJECT="email subject"
MESSAGE="email message"

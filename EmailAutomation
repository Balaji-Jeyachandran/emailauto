import smtplib
from email.mime.text import MIMEText

smtp_server = "smtp.gmail.com"
port = 587
#my password = "gmyu ukyu anzg lbmh"
sender_email = "bmsbalaji80@gmail.com"
receiver_email = "bmsbalaji80@gmail.com"
message = "Hey there!!, this is a automated email using SMTP server"

msg = MIMEText(message)
msg["subject"] = "Hey User!!!!..This is an automated Email"
msg["from"] = sender_email
msg["to"] = receiver_email

password = input("Enter the gmail password : ")

with smtplib.SMTP(smtp_server,port) as server :
    server.starttls()    
    server.login(sender_email, password)
    server.sendmail(sender_email, [receiver_email], msg.as_string())

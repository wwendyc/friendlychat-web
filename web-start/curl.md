curl -H "Content-Type: application/json" \
     -H "Authorization: key=YOUR_SERVER_KEY" \
     -d '{
           "notification": {
             "title": "New chat message!",
             "body": "There is a new message in FriendlyChat",
             "icon": "/images/profile_placeholder.png",
             "click_action": "http://localhost:5000"
           },
           "to": "d5EjrvN9g5o:APA91bEXhRMtE-aBApU3WmjtC8PPETvk1dBou9kqQeCm-aZRYp65osPTevovFu1J5FGAe-v3_6JRF2mSIkGn8j_-hAUmL4UdCyAmGcPDZRjpLpU78ZefV8MlXoKI_yPAmHR0Pgt4LX3Q"
         }' \
     https://fcm.googleapis.com/fcm/send

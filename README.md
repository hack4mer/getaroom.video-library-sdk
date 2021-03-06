# Getaroom.video Library SDK
Getaroom.video library SDK - Guide to implementing a QR scanner in your own app to play videos on getaroom

- Step 1: Implement a QR scanner in your application (you can user any library or sdk)
- Step 2: When user scans the QR code at getaroom.video library, they get a websocket url like this: `wss://connect.websocket.in/getaroomdotvideo?room_id=2`
- Step 3: Connect to this websocket url
- Step 4: Send a JSON payload on the socket connection,
 Payload format: 
        
        {
            "key":"library",
            "value":"https://sample-videos.com/video123/mp4/720/big_buck_bunny_720p_1mb.mp4"
        }
- As soon as you send the payload, the video link is loaded in the user's getaroom.video player.

## Apps that implement this SDK:
- [SuperFlix](https://superflix.co)


Note: If you have implemented Getavideo.room library SDK in your application, you can add your application link in this repository. Simply, make a pull request for us to merge.

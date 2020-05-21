# Serverless WebRTC
To establish a P2P connection without a signalling server you have to exchange the SDPs between your clients (local and remote). Try it out. Open the [demo](https://maiermic.github.io/serverless-webrtc/webrtc-noserver.html) in two tabs or two different devices, lets say client **A** and client **B**.
1. Client **A**
    - click on `createOffer`
    - copy the generated SDP and send it to **B** (e.g. using email)
2. Client **B**
    - paste SDP of **A** (e.g. received by email) in (**B**'s) text box `Remote`
    - click `answer` button (this will generate another SDP and add it to text box `Local`)
    - copy the generated SDP (of text box `Local`) and send it to **A** (e.g. using email)
3. Client **A**
    - paste SDP of **B** (e.g. received by email) in (**A**'s) text box `Remote`
    - click `answer` button
Now you should be able to see P2P connection working.

## features
* peer to peer video calling
* chat
* file transfer

## Snap
![serverless-webrtc](snap.png)

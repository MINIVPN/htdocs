# CHAT ONLINE!
<html>
<head>
    <title>Online Chat</title>
    <style>
        .chat-box {
            width: 300px;
            height: 200px;
            overflow-y: scroll;
        }

        .message {
            margin-bottom: 5px;
        }
    </style>
</head>
<body>
    <div class="chat-box" id="chat-box"></div>
    <input type="text" id="messageInput" placeholder="Enter your message...">
    <button onclick="sendMessage()">Send</button>
    <button onclick="clearMessages()">Clear</button>

    <script>
        var username = "guest" + Math.floor(Math.random() * 1000);
        
        function sendMessage() {
            var message = document.getElementById("messageInput").value;
            
            var newMessage = document.createElement("div");
            newMessage.className = "message";
            newMessage.textContent = username + ": " + message;

            document.getElementById("chat-box").appendChild(newMessage);
            document.getElementById("messageInput").value = "";
        }

        function clearMessages() {
            if(username === "Admin") {
                document.getElementById("chat-box").innerHTML = "";
            } else {
                alert("You are not authorized to clear messages.");
            }
        }
    </script>
</body>
</html>

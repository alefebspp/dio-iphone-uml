classDiagram
    class iPhone {
        +makeCall(phoneNumber: String)
        +takePhoto()
        +sendMessage(contact: String, message: String)
    }

    class Phone {
        +dialNumber(phoneNumber: String)
        +endCall()
    }

    class Camera {
        +openCamera()
        +capturePhoto()
        +closeCamera()
    }

    class Messages {
        +composeMessage(contact: String, message: String)
        +sendMessage(contact: String, message: String)
        +receiveMessage(contact: String, message: String)
    }

    iPhone --> Phone
    iPhone --> Camera
    iPhone --> Messages

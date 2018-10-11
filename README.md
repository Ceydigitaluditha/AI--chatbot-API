# AI- chatbot API


# APIs

> GET /user    

    Get  "index.html" File

> GET /qrcode

    Redirect to play.google.com or itunes.apple.com according to OS type

> GET /user/privacy
    
    GET user privacy details

> POST /user/update

    Update user's name,image and status.

> POST /user/getOTP

    Given mobile number and country code, This API generates OTP And sends it to the user.

> POST /user/register 
    
    To register a new user.

> POST /channel/getChannelParticipants

    GET channel participants list by "channelId"

> POST /group/getGroupParticipants
    
    Get group participants

> POST /group/updateName

    Update group name

> POST /group/updateImage

    Update group image

> POST /group/addParticipants

    Add participants to a group

> POST /user/syncContacts

    To sync and display registered contacts in the app.

> POST /user/acceptCall

    To accept an incoming call which will send a push notification to the caller.

> POST /user/endCall

    To end an ongoing call.

> POST /user/voiceCall

    To place an outgoing call.

> POST /user/updateRecoveryDetails
    
    Update user's recovery details.

> POST /user/updatePrivacySettings

    Update user's privacy settings.

> POST /user/checkRecoveryDetails

    Check user's recovery details

> POST /user/requestOtp

    For changing chatlock password

> POST /user/voipPush

    Send request to terminate application 

# Admin


> POST /admin/login

    Send login request

> GET /admin/dashBoard

    Get text,image,video,audio,location,sticker,contact,android,ios count

> GET /admin/userList

    Get all users with friends count,group count

> GET /admin/groupList

     Get all groups list

> POST /admin/myGroups

    SET "userId" to payload

> POST /admin/groupsIOwn

    Get groups list with name,image,id,groupId,createdBy,createdById,
    createdAt details that created by the request "userId" 

> POST /admin/groupMembers

    SET "groupId" to payload

> POST /admin/groupParticipants

    Get all the group participants details by the request "groupId"

> POST /admin/updateProfile

    Update profile 

> POST /admin/userFriends

    Get user friend list with name,status,image and id 

> POST /admin/groupProfile

    Get group profile details with total member count by the request "groupId" 

> POST /admin/userProfile

    Get user profile details with friend list


# Socket.io

> disconnect

    Log "A socket with sessionID ${sessionID} disconnected!"

> qridemit
    
    Generate QR code

> webonline

    Update user status as web online 

> weboffline

     Update user status as web offline and lastSeen time

> online

    Update user status as online

> offline

    Update user status as web offline and lastSeen time

> typing 

    Display user status as typing in room


> editGroupImage

    Update group image

> deleteFromCache

    Delete From Cache

> editGroupName

    Update group name

> removeAdmin

    Update group participant admin status as false

> makeAdmin

    Update group participant admin status as true

> removeParticipant

    Remove participant from group

> exitGroup

     Remove group
    
> addParticipants

    Add participant to a group

> exitChannel

    Remove participant from a group

> removeParticipantInChannel

    Remove participant from a channel

> removeAdminInChannel

    Remove admin access and set as "user"

> addAdminInChannel

    Set participant as a admin in a channel

> editChannel

    Update channel details

> createChannel

    Create new channel

> createGroup

     Create new group

> getOnline
    
    Send online status

> ack

    Removes the specified fields (userid,messageid) from the hash stored at key. Specified 
    fields that do not exist within this hash are ignored. 
    
    If key does not exist,it is treated as an empty hash and this command returns 0

> sendDelivered

    Send message status as delivered 

> sendSeen

     Send message status as seen

> sendBroadcast
    
    Send broadcast message

> sendMessageInChannel

    Send message in a channel

> sendMessage

    Send message in a group chat
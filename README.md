### How To Use App API

### http://localhost:3000/api/verify/sendsms

**Args**

Method : Post </br>
Input : [PhoneNumber]: Number </br>
Return : [Request_id] in case success otherwise return error message </br>

############################################

### http://localhost:3000/api/verify/check

**Args**

Method : Post </br>
Input : [PhoneNumber]: Number,[Request_id]:id,[Code]:code that send to user via sms </br>
Return : List Of Temp Id [100] in case success otherwise return error message </br>

**Note**

Above I Combine Check Validation And Insert User In One Function </br>

############################################

### http://localhost:3000/api/getGenerateIds

**Args**

Method : Post </br>
Input : [tempId] : id </br>
Return : List Of Temp Id [100] in case success otherwise return error message </br>

############################################

### http://localhost:3000/api/getHandshakePin

**Args**

Method : Get </br>
Input : Nothing </br>
Return : [Pin] Used For Get The Upload Token </br>

############################################

### http://localhost:3000/api/getUploadToken

**Args**

Method : Post </br>
Input : [tempId] : id , [pin]: pin That You Receiving Before From Get [getHandshakePin] API</br>
Return : [token] Used For Upload File For Security Reasons </br>

############################################

### http://localhost:3000/api/upload

**Args**

Method : Post </br>
Input : [File] : FileData ,[token]:token </br>
Return : [success] otherwise return error message </br>

############################################

**Note**

We finished backend And Frontend Dashboard Just You Need To Have An Account To Access The Dashboard Page [http://localhost:3000/] ... </br>
so, We Should To Run [setup.js] File To Create Admin Account On The Database Before Access Dashboard.. </br>

To Run File Use [ **Node setup.js** ] In The Current Directory Of The Project
#   M i n i P r j B r  
 #   M i n i P r j B r  
 
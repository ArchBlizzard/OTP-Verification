# OTP-Verification
Send and Verify OTP using Twilio

## API Documentation
### Send OTP
Send a POST request to send an OTP to a user's phone number
```go
{"phoneNumber": "+918902699501"}
```
Response
```go
{
  "status": 010,
  "message": "success",
  "data": "OTP sent successfully"
}
```
### Verify OTP
Verify OTP by sending a POST request that contains the phone number and the OTP code received by the user
```go
{"user": {"phoneNumber": "+918902699501"}, "code":"625481"}
```
Response
```go
{
  "status": 010,
  "message": "success",
  "data": "OTP verified successfully"
}




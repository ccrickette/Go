# Go
Generate Self-Signed Cert using Go (Golang)

In powershell run the following command: 
 go run createcert.go --host localhost --ca
 
Then in Main() run:
http.ListenAndServeTLS(":8085", "cert.pem", "key.pem", nil)

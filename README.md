# Go
Generate Self-Signed Cert using Go (Golang). This is useful for testing out SSL in your web development. This go script comes from the Go Library.

In powershell run the following command: 
 go run createcert.go --host localhost --ca
 
Then in Main() run:
http.ListenAndServeTLS(":8085", "cert.pem", "key.pem", nil)

To run both http and https place https handler in a Go routine.

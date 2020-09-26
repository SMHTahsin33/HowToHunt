
Hello I Have Provided Some Testing Methods and Bypasses Methods On SSRF Below

- **Server Side Request Forgery(SSRF)**
- Use The Whole IP Range For Testing SSRF (198.0.0.1-255)
- Use Different Encoding Schemes of https://127.0.0.1
    Hex Encoding ==> https://0x7f.0x0.0x0.0x1
    Octal Encoding ==> https://0177.0.0.01
    Dword Encoding ==> https://2130706433
    URL Encoding ==> https://%6c%6f%63%61%6c%68%6f%73%74
    Mixed Encoding ==> https://0177.0.0.0x1
    Also use `2130706433` or `017700000001`
- Obfuscate Strings In URL Encode or Case Transformation (Blocked Words Bypass)
- Use Registered Domain Names That Resolves To 127.0.0.1
- Embed Credentials : https://attacker@victim.com
- Use URL Fragments '#' : https://attacker'#'victim.com (Remome the '' over the hash)
- Use DNS Subdomain Method : https://victim.com.evil.com
- Use Directory Method : https://attacker.com/victim.com
- Exploit Redirecting The Target
- Change The Referrer To Burp Collaborator [Blind Exploit]
- Use IPv6 addresses instead of IPv4
- Usable Protocols:
    `gopher://`
    `file://`
    `dict://`
    `sftp://`


Twitter: @smhtahsin33

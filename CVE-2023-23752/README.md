# CVE-2023-23752 - Joomla Information Disclosure

Yo, I needed to use this exploit in a HTB machine and the only other PoC I could find was written in ruby...

I didn't wanna mess with the ruby dependancies so I just re-wrote it in python "real quick".

---
This is basically just a parser for the JSON returned by the open API endpoints, this can be replicated easily with CURL or a web browser by hitting the following endpoints:

#### User Info

`/api/index.php/v1/config/applicaton?public=true`

#### Config Info

`/api/index.php/v1/config/application?public=true"`

## Usage
`python3 CVE-2023-23752.py -t <target_url>`

---


# License
GPL v3.0 - as all good software should be

Remember - don't be a skid :)

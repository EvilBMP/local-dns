# Public wildcard domains pointing to localhost:


| URL                   | Target                | Notes               |
|-----------------------|-----------------------|---------------------|
| *.127-0-0-1.org.uk    | 127.0.0.1             |                     |
| *.ddev.site           | 127.0.0.1             |                     |
| *.lacolhost.com       | 127.0.0.1             |                     |
| *.localtest.me        | 127.0.0.1             | Except [readme.localtest.me](readme.localtest.me) |
| *.localhost.tv        | 127.0.0.1             | Except localhost.tv |
| *.localhst.co.uk      | 127.0.0.1             |                     |
| *.lvh.me              | 127.0.0.1             |                     |
| *.vcap.me             | 127.0.0.1             |                     |


# Public wildcard domains pointing to any IP address:

* magic DNS services that, when queried with a hostname and with an embedded IP address, return that IP address

| URL                   | Example -> Target     | Note                |
|-----------------------|-----------------------|---------------------|
| *.nip.io              | <ul><li>`10.0.0.1.nip.io` maps to `10.0.0.1`</li><li>`192-168-1-250.nip.io` maps to `192.168.1.250`</li><li>`domain.tld.192.168.1.1.nip.io` maps to `192.168.1.1`</li></ul> | nip.io maps `<anything>[.-]<IP Address>.nip.io` in either **"dot"** or **"dash"** notation to the corresponding `<IP Address>`<br/><br/>More information on [nip.io](nip.io) |
| *.sslip.io              | <ul><li>`10.0.0.1.nip.io` maps to `10.0.0.1`</li><li>`192-168-1-250.nip.io` maps to `192.168.1.250`</li><li>`domain.tld.192.168.1.1.nip.io` maps to `192.168.1.1`</li><li>`–1.sslip.io` maps to `::1`</li><li>`2a01-4f8-c17-b8f--2.sslip.io` maps to `2a01:4f8:c17:b8f::2`</li></ul> | sslip.io maps `<anything>[.-]<IP Address>.sslip.io` in either **"dot"** or **"dash"** notation to the corresponding `<IP Address>`<br/><br/>IPv4 and IPv6 support<br/><br/>More Information on [sslip.io](sslip.io) |
| *.xip.io              | <ul><li>`10.0.0.1.xip.io` maps to `10.0.0.1`</li><li>`domain.tld.192.168.1.1.xip.io` maps to `192.168.1.1`</li></ul> | xip.io maps `<anything>[.]<IP Address>.xip.io` in **"dot"** notation to the corresponding `<IP Address>`<br/><br/>More Information on [xip.io](xip.io) |

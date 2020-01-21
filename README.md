# dnssec
Get DNSSEC info of a domain

Check cmd folder for example usage.

Output:

```json
{
  "domain": "binaryfigments.com",
  "answer": {
    "dsrecordcount": 1,
    "dnskeyrecordcount": 4,
    "dsrecords": [
      {
        "algorithm": 7,
        "digest": "403cc33ad60d52ad254607bd1c5fdcaf0020574e",
        "digesttype": 1,
        "keytag": 52653
      }
    ],
    "dnskeyrecords": [
      {
        "algorithm": 7,
        "flags": 256,
        "protocol": 3,
        "publickey": "AwEAAaIRIN0VPYdqbRI8i6zh6tmsIwf424VffKh7qeROoFoJ04AIl1KjV+unBa1hUgq0N25vhO1kpn3NDmyhvQhvNIq9M/MBJUmTucw3THpDHCUVpJsH4PrWVnEA5rkBjXy6guuSIl1GeUqXX9A0jL36yHs1vdph8mSxV36g0JHzVYiv"
      },
      {
        "algorithm": 7,
        "flags": 256,
        "protocol": 3,
        "publickey": "AwEAAegiFnEctYZ7OBENzucs4Lno/sJWr4lzPB9EkPzOVovrSBlbFWzjR2vd92vx13/vD5PtNmJ1PRz+0z74Y7Y2gIs+aS5RmE/co0zlMwhaYmuqeEO+HRzDxeSsDJoFToUy72tPT812sjQWOvfuiDuYphyicHcwdGkGNI3c0qP3Otlh"
      },
      {
        "algorithm": 7,
        "flags": 257,
        "protocol": 3,
        "publickey": "AwEAAd91QIVUw9qyE2UWyAY3IeWEwiGfhUwXBGvVa3GSnK5maQ0PzHJikmjeCfvyx+y13SJCopHxF1nXCaU9BXw7soriYpfI3V59ypuLVcy0iAzsZyyIpeVDyVsCbiCZJ7CNc6WlbC83JYaRVy5auRLFLslJKeAqQthKqgAXv05IPT5Syq+GQNre2G7fDZgzvv3A9ZIZyAGYfIWHqOHmw271tC6wOa9BzCenmK8dgRWMTO7Pc7OoqKEM42xjXlDqPX8I9SRV2w11/FRR3LquCuLft9OlRY9GMMxF7DmiEoyP1IdZzF+/yQhggvWE2OEcbIkU5rQIuCDzVTSOOjZE6+P3fHE="
      }
    ],
    "calculatedds": [
      {
        "algorithm": 7,
        "digest": "403cc33ad60d52ad254607bd1c5fdcaf0020574e",
        "digesttype": 1,
        "keytag": 52653
      },
      {
        "algorithm": 7,
        "digest": "1520f289eb26e138c380cdf3f460927101f727f9",
        "digesttype": 1,
        "keytag": 22802
      },
      {
        "algorithm": 7,
        "digest": "4c4e590562683c5b00761cd7aaa308f4b0eeb4e8",
        "digesttype": 1,
        "keytag": 38087
      }
    ],
    "matching": {
      "ds": [
        {
          "algorithm": 7,
          "digest": "403cc33ad60d52ad254607bd1c5fdcaf0020574e",
          "digesttype": 1,
          "keytag": 52653
        }
      ],
      "dnskey": [
        {
          "algorithm": 7,
          "flags": 256,
          "protocol": 3,
          "publickey": "AwEAAaIRIN0VPYdqbRI8i6zh6tmsIwf424VffKh7qeROoFoJ04AIl1KjV+unBa1hUgq0N25vhO1kpn3NDmyhvQhvNIq9M/MBJUmTucw3THpDHCUVpJsH4PrWVnEA5rkBjXy6guuSIl1GeUqXX9A0jL36yHs1vdph8mSxV36g0JHzVYiv"
        }
      ]
    }
  },
  "time": "2020-01-21T21:57:20.754828848+01:00",
  "dnssec": true,
  "nsec": {
    "type": "nsec3param",
    "nsec3param": {
      "Hdr": {
        "Name": "binaryfigments.com.",
        "Rrtype": 51,
        "Class": 1,
        "Ttl": 0,
        "Rdlength": 13
      },
      "Hash": 1,
      "Flags": 0,
      "Iterations": 100,
      "SaltLength": 8,
      "Salt": "5db86ef2e91811ad"
    }
  }
}
```
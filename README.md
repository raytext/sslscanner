# sslscanner

TODO: Write a description here

## Installation

Add this to your application's `shard.yml`:

```yaml
dependencies:
  sslscanner:
    github: bararchy/sslscanner
```

## Usage

```crystal
require "sslscanner"
# This will start a scan of google.com
scanner = SSLScanner::Scan.new("google.com", 443)
scanner.run
```

Or you can use the example under /bin

```bash
crystal build bin/scan.cr --release
./scan google.com 443
```

## Development

- [ ] Add more issues (SSL Issues)  
- [x] Multiscanning (using fibers)  
- [ ] Export results to pdf\txt\csv\etc..  
- [ ] Add local OpenSSL installation with all ciphers enabled so we don't need to relay on system openssl  
- [ ] Add more checks: HeartBleed, compression, renegotiation, etc..  

## Contributing

1. Fork it ( https://github.com/bararchy/sslscanner/fork )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create a new Pull Request

## Contributors

- [bararchy](https://github.com/bararchy) - creator, maintainer

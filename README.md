# cosign
Sigstore cosign repository for Home Assistant


## Binary

Binary files for our Alpine Linux based Docker images.
Prebuild for speed-up the build process.

Source: https://github.com/sigstore/cosign/releases

Commands:

- CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build -trimpath -o cosign_amd64 ./cmd/cosign
- CGO_ENABLED=0 GOOS=linux GOARCH=386 go build -trimpath -o cosign_i386 ./cmd/cosign
- CGO_ENABLED=0 GOOS=linux GOARCH=arm GOARM=7 go build -trimpath -o cosign_armv7 ./cmd/cosign
- CGO_ENABLED=0 GOOS=linux GOARCH=arm GOARM=6 go build -trimpath -o cosign_armhf ./cmd/cosign
- GO_ENABLED=0 GOOS=linux GOARCH=arm64 go build -trimpath -o cosign_aarch64 ./cmd/cosign

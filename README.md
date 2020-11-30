# File share

File share server is a file sharing service as well as can act as file storage. This project is to provide flexible auth options, support multiple storage options available along with providing the basic file operation like upload a file, share a file, delete a file.

## Features 

- Presigned link generation for upload, download operation with specific criteria like time bound link, one time use
- Ablilty to validate the presigned operation using custom auth schemes
- Project based configuration

## Why this project?

While working on [Vartalap](https://vartalap.one9x.com), in order to implement features like profile pic, file sharing, a file server is required. Current vartalap server are not powerful enough to support another service like file(upload, downloads). So it is decided to use external service for file operations while maintaining the security, although there are number of  storage options like AWS S3, Azure storage but none of the service provides custom auth. One solution is to perform auth on [Vartalap](https://vartalap.one9x.com) server and then redirect them to desire service, but that will defeat the purpose as vartalap server is not that powerful to handle more external requests.


## Resources

- Open api - [docs/openapi.yml](docs/openapi.yml)


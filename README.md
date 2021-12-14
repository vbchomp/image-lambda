# image-lambda

## Version 1.0.00

## Deployed Sites

- [steven-tyler-pjs bucket](https://s3.console.aws.amazon.com/s3/buckets/steven-tyler-pjs?region=us-east-2&tab=objects)

- [github](https://github.com/vbchomp/image-lambda)

## Author

Heather Bisgaard, Software Engineer

## Collaborators

Whole class during review

## References

- AWS Docs

## Set Up Notes

1. Created a bucket named steven-tyler-pjs and uploaded an image on S3. Opened permissions to public so anyone can view.

2. Read image data and write the body into the buffer. This is where the issues happened when writing to the buffer.

3. Create meta data.

4. Then re-upload to AWS S3.

## Issues

Everything else in lab seemed to work and apparently all that is needed is the buffer part to work. However, we would get errors when trying to write to the buffer. In class, then re-watching the video showed that the write() only returns an integer. Not sure why it would only return an integer when we were trying to get a response assigned to it.

They tried stringifying the body, then parsing the body and nothing ended up working. Even with the demo code that was out of date. So Alex suggested we just submit talking about what happened in class.

# Interviews

## resources

- [https://github.com/kdn251/interviews](https://github.com/kdn251/interviews)

- [5 Salary Negotiation Rules for Software Developers](https://dev.to/aershov24/5-salary-negotiation-rules-for-software-developers-get-20-on-top-of-your-market-rate-2jii)


## Some interview questions

### Why ssd is faster than hdd

One is that compared to a spinning hard disk the access (seek) time is miniscule, the hard disk needs to move the head to the right track and then wait for the sector to be under the head (depends on rotation speed) this is on average about 10 milliseconds. The SSD on the other hand needs to send a command to the flash chip on a fast interconnect and data will stream back in a few microseconds.

The other factor is parallelism, the HDD has a single head construction and it can only read from one head at a time so if you send it 32 commands at the same time the last one will only be started after all the others have completed (assuming no reordering). The SSD can access multiple flash chips at the same time and order them all to fetch data, it can even pull the data to its own RAM in parallel from multiple flash chips, most consumer SSDs can handle at least 8 requests in parallel so it can be blazing fast. This is also the different between the SSD and a USB flash drive, the USB flash drive only has one flash chip so it has no parallelization.

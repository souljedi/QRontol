# QRontol
Control stuff via QR codes.

The main goal of this project is to provide a tangible interface to trigger user-defined actions. While not meant to completly replace other interfaces, this is meant to provide an alternative interaction metaphor for certain actions. The inspiration came from the "old analog way" of browsing for music, e.g., flipping through some LP or CD albums covers in a box. This directly leads to one use cases, printing out and laminating QR coded cards with album art. In this case, one can literally browse through a deck of cards and hand pick an album. The selected card can be scanned, which triggers an action that starts the playlist on a streaming music service or starts the album in a local mp3 player etc. The system can be potentially also used by small kids, without having to navigate any menues or getting distracted by other apps on a phone or tablet.

# System overview
* QR code card generator: svg-template and python script
  * the script will autogenerate QR codes and register them with the command server (see below),
  * populate the svg file, e.g., based on some csv input file, or using some scraper
  * the svg file, can be converted to a PDF and then be printed and laminated by the user
* QR code reader:
  * generic reader: any QR reader app on a smartphone; reads an URL from the QR code, that triggers via a webhook the command server
  * custom reader: runs on a dedicated device, e.g., [octocam](https://shop.pimoroni.com/products/octocam-pi-zero-w-project-kit); reads a numeric sequence from the QR code and pass it on to the command server
* command server: implemented in python
  * has a database of QR codes associated with actions
  * receives a decoded QR code and triggers a command/action of a third party API

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Give examples
```

### Installing

pip integraton is planed for later and will be documented here.

A step by step series of examples that tell you have to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/souljedi/QRontol/tags). 

## Authors

* **Sebastian Ullrich** - *Initial work* - [souljedi](https://github.com/souljedi)

See also the list of [contributors](https://github.com/souljedi/QRontol/graphs/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* **Billie Thompson** - For the Readme and contributing templates - [PurpleBooth](https://github.com/PurpleBooth)
* Inspiration
* etc

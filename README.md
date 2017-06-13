# QRontol
Control stuff via QR codes, that trigger python scripts.

The main idea is to provide a tangible interface to control user-defined actions, e.g., as an alternative to a touch screen interface. The inspiration comes from the "old way" of browsing for music, e.g., by flipping through some LP or CD albums covers in a box. So one of the use cases is to create/print album QR cards, e.g., having a set of cards with QR codes on them. Then one can browse through the deck of cards and pick an album, scan it which triggers an action that starts the playlist on a streaming music service or starts the album in a local mp3 player etc. 

# System overview
* printed QR code tags
* QR code reader which either is a
  * custom reader: interprets the code and triggers a command or
  * generic reader: visits a special URL, that triggers a command elsewhere
* command server: receives command and triggers a command/action at any third party API

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Give examples
```

### Installing

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

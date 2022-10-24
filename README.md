mkdigauth
=========

By Rémino Rem <https://remino.net/>

Create digest auth .htdigest file for Apache HTTPd with related .htaccess file.

[Code & Download](https://github.com/remino/mkdigauth/)

- [Getting Started](#getting-started)
	- [Installation](#installation)
		- [Using Homebrew on macOS](#using-homebrew-on-macos)
		- [Using git](#using-git)
		- [Using cURL](#using-curl)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)



## Getting Started

### Installation

#### Using Homebrew on macOS

```sh
brew tap remino/remino
brew install mkdigauth
mkdigauth -h
```
#### Using git

```sh
git clone https://github.com/remino/mkdigauth.git
cd mkdigauth
./mkdigauth -h
```

#### Using cURL

```sh
curl -L https://github.com/remino/mkdigauth/raw/main/mkdigauth > mkdigauth
chmod +x mkdigauth
./mkdigauth -h
```

[Back to top](#mkdigauth)



## Usage

```
mkdigauth 1.0.0

USAGE: mkdigauth [-ahprtuv] [<outputdir>]

Create digest auth .htdigest file for Apache HTTPd with related .htaccess file.

Will output to current directory if no outputdir is specified.

OPTIONS:

	-a        Specify absolute path base to .htdigest file to use.
	          Path will become <pathbase>/<outputdir>/.htdigest.
	          If not specified, will only <outputdir>/.htdigest.
	          (Note AuthUserFile in .htdigest cannot be relative.)
	-c        Clear all output files in <outputdir> before processing.
	-h        Show this help screen.
	-p        Specify password instead of generating one.
	-r        Specify realm. (Default: Access)
	-s        Show password on report.
	-T        Omit .htaccess file.
	-u        Specify username. (Default: user)
	-v        Show script name and version number.

```

[Back to top](#mkdigauth)



## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

[Back to top](#mkdigauth)



## License

Distributed under the ISC License. See `LICENSE.txt` for more information.

[Back to top](#mkdigauth)

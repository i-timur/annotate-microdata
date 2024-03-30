<a name="readme-top"></a>

# Annotate with microdata

## About the project

This project aims to provide a simple way to annotate HTML with microdata by utilizing *Deep Learning* methods.

The main motivation behind this project is to manage the tedious task of annotating HTML with microdata. Microdata is part of the WHATWG HTML Standard and is used to nest metadata within existing content on web pages. Search engines greatly benefit from microdata and boost web pages in search results.

This project is made as part of thesis work in Institute of Information Technologies and Intelligent Systems for a bachelor's degree

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Getting started

### Prerequisites

- Python 3.9.6+
- pip 24.0+
- python3-virtualenv if running Linux

### Installation

- Clone repository
  ```shell
  git clone git@github.com:i-timur/annotate-with-microdata.git
  ```
- Setup virtual environment
  - MacOS
    ```shell
    python3 -m venv venv
    source venv/bin/activate
    ```
  - Windows
    ```shell
    python3 -m venv venv
    .\venv\Scripts\activate
    ```
  - Linux
    ```shell
    virtualenv venv
    source venv/bin/activate
    ```
- Install dependencies
  ```shell
  pip install -r requirements.txt
  ```
- Install the package globally
  ```shell
  pip install -e .
  ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage

### Annotate HTML with microdata

Annotate HTML with microdata by passing HTML directly to the shell command

```shell
microdata --inline '<YOUR_HTML>'
```

or by passing a file with HTML

```shell
microdata --filepath <PATH_TO_FILE>
```

Before passing HTML, make sure that the HTML is valid and **wrapped with `<body>` tag**.

Set output file with `--output` flag

```shell
microdata --inline '<YOUR_HTML>' --output <OUTPUT_FILE>
```

Following entities are currently supported:
- [X] Product
- [X] Book
- [X] Event
- [X] Hotel
- [X] JobPosting
- [X] Movie
- [X] Recipe
- [X] Restraurant
- [ ] Organization
- [ ] Place
- [ ] Person
- [ ] PostalAddress
- [ ] Creative Work
- [ ] LocalBusiness
- [ ] Painting

## Roadmap

- [ ] Add HTML validation
- [ ] Add support for JSX syntax

See the [open issues](https://github.com/i-timur/annotate-with-microdata/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contact

Timur - [Telegram](https://t.me/i_timur) - [i.timur0701@gmail.com](mailto:i.timur0701@gmail.com)

Project Link: [https://github.com/i-timur/annotate-with-microdata](https://github.com/i-timur/annotate-with-microdata)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Acknowledgments

- [web-segment](https://github.com/liaocyintl/web-segment)
- [bert-multilingual](https://github.com/google-research/bert/blob/master/multilingual.md)
- [Best-README-Template](https://github.com/othneildrew/Best-README-Template)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

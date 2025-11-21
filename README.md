<div id="top"></div>
<!-- PROJECT LOGO -->
<br />
<div align="center">
<h3 align="center">Goat co</h3>

  <p align="center">
    This repo serves as a base for goat-co source code.
    <br />
    <a href="https://github.com/tbaledent/goat-co"><strong>Explore the repo »</strong></a>
    <br />
    <br />
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

WIP


<p align="right">(<a href="#top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

### Prerequisites
(only for local development)

<p align="right">(<a href="#top">back to top</a>)</p>

### Installation

This project uses a combination of asdf and direnv to manage dependencies and get your local environment setup to run Airflow locally.
Follow these steps to get your local environment up and running:
1. Clone the repo
   ```sh
   git clone git@github.com:tbaledent/airflowdev.git
   ```
2. Install required dependencies
   ```sh
   brew install postgresql
   brew install asdf
   ```
3. Install asdf plugins
   ```sh
   asdf plugin-add python
   asdf plugin-add direnv
   asdf install python 3.9.5
   asdf install direnv 2.30.3
   asdf global python 3.9.5
   asdf global direnv 2.30.3
   ```
5. Export values to `~/.zshrc` file
   ```sh
   echo 'export PATH="/opt/homebrew/bin:$PATH"' >> ~/.zshrc
   echo 'export PATH="$HOME/.asdf/shims:$PATH"' >> ~/.zshrc 
   echo 'export HOMEBREW_NO_AUTO_UPDATE=1' >> ~/.zshrc
   echo 'eval "$(asdf exec direnv hook zsh)"' >> ~/.zshrc
   echo -e "\n. $(brew --prefix asdf)/libexec/asdf.sh" >> ~/.zshrc
   ```
6. Activate virtual environment & install packages
   ```sh
   source ~/.zshrc
   cd airflowdev
   asdf direnv allow
   make install
   pre-commit install
   ```
7. Create a `.envrc` file at project root and copy contents of `.envrc.sample`
to newly created `.envrc` file.

<p align="right">(<a href="#top">back to top</a>)</p>

## Usage
WIP

<p align="right">(<a href="#top">back to top</a>)</p>

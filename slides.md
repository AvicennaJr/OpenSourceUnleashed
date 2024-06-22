---
theme: seriph
background: https://cover.sli.dev
title: NURU PROGRAMMING LANGUAGE 🔥
info: |
    A Swahili Programming Language of its kind built from the ground up.

    https://nuruprogramming.org

class: text-center
highlighter: shiki
drawings:
    persist: false
transition: slide-left
mdc: true
---

# NURU PROGRAMMING LANGUAGE 🔥

A Swahili Programming Language of its kind built from the ground up.

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/nuruprogramming/nuru" target="_blank" alt="GitHub" title="Open in GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---
transition: none
---

# Why Nuru 🔥?

## Removing the English Barrier

Programming is a universal skill, but the need for proficiency in English has often been a stumbling block for many. Nuru intends to remove this barrier. It allows individuals to grasp programming concepts without the prerequisite of English proficiency.

We believe in democratizing programming knowledge.

---
transition: none
---

# Why Nuru 🔥?

## Preserving Cultural Heritage

There is no rule that all programming languages must be made in English. And Swahili being the most prominent language in East Africa, having a __Swahili Programming Language__ leaves our mark in the global landscape.

---
layout: image-right
image: ./it_aint_much.png
---

# Why Nuru 🔥?

## To Inspire People In Our Community

There are many individuals doing inspiring work in the developer community. Their work has inspired and motivated me. And I hope that this project will inspire more people, show them what's possible and for them to realize there's nothing no limit to what we can build.

---
transition: none
---

# Why Nuru 🔥?

## Why Not

---
transition: none
---

# What Nuru Is Not

## A Replacement For Existing languages

It doesn't intend to compete with any other existing language such Go, Python and so on

## A Translation Or Transpiler

It is not a transalation of any existing language such as Go, Python and so on. It is, however, written in Go same way python is written in C.

## To Be Used In Production

Just don't use it in Production unless you do not fear death.

---
transition: none
layout: image-right
image: ./nuru_works.svg
---

# How Nuru Works

- Token creation (define our terms)
- Lexer (forms the syntax)
- Parser (check syntax)
- Evaluation
- Installers (github Actions)

---
transition: none
class: text-center
---

# Getting Started With Nuru 🔥

---
transition: none
---

## Installation

To get started download the executables from the release page or follow the instructions for your device below:

### Linux

 - Download the binary:

```bash
curl -O -L https://github.com/NuruProgramming/Nuru/releases/download/v0.5.16/nuru_Linux_amd64.tar.gz
```

  - Extract the file to make global available:

```bash
sudo tar -C /usr/local/bin -xzvf nuru_Linux_amd64.tar.gz
```

 - Confirm installation with:

```bash
nuru -v
```

---
transition: none
---

### MacOs ( Apple silicon Mac )

- Download the binary:

- For apple silicon mac use:

```bash
curl -O -L https://github.com/NuruProgramming/Nuru/releases/download/v0.5.16/nuru_Darwin_arm64.tar.gz
```

- For apple intel mac use:

```bash
curl -O -L https://github.com/NuruProgramming/Nuru/releases/download/v0.5.16/nuru_Darwin_amd64.tar.gz
```

- Extract the file to make global available:
- For apple silicon mac use:

```bash
sudo tar -C /usr/local/bin -xzvf nuru_Darwin_arm64.tar.gz
```
- For apple intel mac use:

```bash
sudo tar -C /usr/local/bin -xzvf nuru_Darwin_amd64.tar.gz
```

- Confirm installation with:

```bash
nuru -v
```

---
transition: none
---

### Android (Termux)

 - Make sure you have [Termux](https://f-droid.org/repo/com.termux_118.apk) installed.
 - Download the binary with this command:

```bash
curl -O -L https://github.com/NuruProgramming/Nuru/releases/download/v0.5.16/nuru_Android_arm64.tar.gz
```
 - Extract the file:

```bash
tar -xzvf nuru_Android_arm64.tar.gz
```
 - Add it to path:

```bash
echo "alias nuru='~/nuru'" >> .bashrc
```
 - Confirm installation with:

```bash
nuru -v 
```

---
transition: none
---

### Windows

- Download the Nuru zip file [Here](https://github.com/NuruProgramming/Nuru/releases/download/v0.5.16/nuru_Windows_amd64.zip)
- Unzip to get the executable
- Double click the executable

---
transition: none
---

### Building From Source

- Make sure you have golang installed (atleast 1.19.0 and above)
- Run the following command:

```bash
go build -o nuru main.go
```
- You can optionally add the binary to `$PATH` as shown above
- Confirm installtion with:

```bash
nuru -v
```

### Many Other Builds

Just visit:

https://github.com/NuruProgramming/Nuru/releases/tag/v0.5.16

---
transition: none
---

## Syntax At A Glance

**NOTE**
> There is a more detailed documentation of the language [here](https://nuruprogramming.org).

Nuru, although still in its early stage, intends to be a fully functional programming language, and thus it has been baked with many features.

---
transition: none
---

### Defining A Variable

You can define variables like this:

```go
x = 2;
y = 3;

andika(x*y) // output is 6
```

You can also use the `fanya` keyword to define a variabe:

```go
fanya x = 3
```

**Note that `fanya` keyword is OPTIONAL**

---
transition: none
---

### Comments

Nuru supports both single line and multiple line comments as shown below:

```go
// Single line comment

/*
Multiple
Line
Comment 
*/ 
```

---
transition: none
---

### Arithmetic Operations

For now Nuru supports `+`, `-`, `/`, `*` and `%`. Nuru also provides precedence of operations using the BODMAS rule:

```go
2 + 2 * 3 // output = 8

2 * (2 + 3) // output = 10
```

---
transition: none
---

### Types in Nuru 🔥

Nuru has the following types:

<table>
  <thead>
    <tr>
      <th>Type</th>
      <th>Syntax</th>
      <th>Comments</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>BOOL</td>
      <td><code>kweli sikweli</code></td>
      <td>kweli == true, sikweli == false</td>
    </tr>
    <tr>
      <td>INT</td>
      <td><code>1, 100, 342, -4</code></td>
      <td>These are signed 64 bit integers</td>
    </tr>
    <tr>
      <td>FLOAT</td>
      <td><code>2.3, 4.5. 100.8094</code></td>
      <td>Signed 64 bit floats</td>
    </tr>
    <tr>
      <td>STRING</td>
      <td><code>"" "mambo" "habari yako"</code></td>
      <td>They can be in double <code>"</code> or single <code>'</code> quotes</td>
    </tr>
    <tr>
      <td>ARRAY</td>
      <td><code>[] [1, 2, 3] [1, "moja", kweli]</code></td>
      <td>Arrays can hold any types</td>
    </tr>
    <tr>
      <td>DICT</td>
      <td><code>{} {"a": 3, 1: "moja", kweli: 2}</code></td>
      <td>Keys can be int, string or bool. Values can be anything</td>
    </tr>
    <tr>
      <td>NULL</td>
      <td><code>tupu</code></td>
      <td>These are nil objects</td>
    </tr>
  </tbody>
</table>

---
transition: none
---

### Functions

This is how you define a function in Nuru:

```
jumlisha = unda(x, y) {
        rudisha x + y
    }

andika(jumlisha(3,4))
```

---
transition: none
---

### If Statements

Nuru supports if, elif and else statements with keywords `kama`, `au kama` and `sivyo` respectively:

```go
kama (2<1) {
    andika("Mbili ni ndogo kuliko moja")
} au kama (3 < 1) {
    andika ("Tatu ni ndogo kuliko moja")
} sivyo {
    andika("Moja ni ndogo")
}
```

---
transition: none
layout: two-cols-header
---

### Arrays

This is how you initiliaze and perform other array operations in Nuru:
::left::
```go
arr = []

// To add elements
sukuma(arr, 2)
andika(arr) // output = [2]

arr2 = [1,2,3,4]

arr3 = arr1 + arr2 // Add two Arrays

andika(arr3) // output = [2,1,2,3,4]
```
::right::
```go
// reassign value

arr3[0] = 0

andika[arr3] // output = [0,1,2,3,4]

// get specific item

andika(arr[3])

// output = 3

```

---
transition: none
---

### Dictionaries

Nuru also supports dictionaries and you can do a lot with them as follows:

```go
mtu = {"jina": "Mojo", "kabila": "Mnyakusa"}
// get value from key 
andika(mtu["jina"]) // output = Mojo
andika(mtu["kabila"]); // output = Mnyakusa

// You can reassign values
mtu["jina"] = "Avicenna"

andika(mtu["jina"]) // output = Avicenna

// You can also add new values like this:
mtu["anapoishi"] = "Dar Es Salaam"

andika(mtu) // output = {"jina": "Avicenna", "kabila": "Mnyakusa", "anapoishi": "Dar Es Salaam"}

// You can also add two Dictionaries
kazi = {"kazi": "jambazi"}

mtu = mtu + kazi
andika(mtu) // output = {"jina": "Avicenna", "kabila": "Mnyakusa", "anapoishi": "Dar Es Salaam", "kazi": "jambazi"}
```

---
transition: none
---

### For Loops

These can iterate over strings, arrays and dictionaries:

```go
kwa i ktk "habari" {
    andika(i)
}
/* //output
h
a
b
a
r
i
*/
```

---
transition: none
---

### Getting Input From User

In Nuru you can get input from users using the `jaza()` keyword as follows:

```go
jina = jaza("Unaitwa nani? ") // will prompt for input

andika("Habari yako " + jina)
```

---
transition: none
---

## How To Run

### Using The Intepreter:

You can enter the intepreter by simply running the `nuru` command:

```go
nuru
>>> andika("karibu")
karibu
>>> 2 + 2
4
```

---
transition: none
---

### Running From File

To run a Nuru script, write the `nuru` command followed by the name of the file with a `.nr` or `.sw` extension:

```bash
nuru myFile.nr
```

---
transition: none
---

## Challenges

- Swahili terminologies: most terminologies are either too hard or non existent
- Testing: As a new programming it needs to be heavily tested by developers to see the limitations and painpoints of the language
- Learning resources: Nuru needs more learning resources that can be easily understood by laymen. Almost all available Nuru resources are for developers.

---
transition: none
---

# How can you help?

## Documentation

There are documentations for two languages, English and Kiswahili, which are both under the `docs` folder. All files are written in markdown. Feel free to contribute by making a pull request.

## Code

Clone the repo, hack it, make sure all tests are passing then submit a pull request.

 > Make sure ALL tests are passing before making a pull request. You can confirm with running `make tests`

## Content

- Blogs and Videos

---
transition: none
---

# The Nuru Community

Nuru has a passionate community, join us on [Telegram](https://t.me/NuruProgrammingChat) or search @NuruProgrammingChat

---
transition: none
layout: two-cols-header
---

## Shoutout To Contributors

Nuru Programming Language has been authored and being actively maintained by [Avicenna](https://github.com/AvicennaJr) and:

::left::

- Victor Kariuki: https://github.com/VictorKariuki
- Lugano Ngulwa: https://github.com/Hopertz
- Karim Nyumba: https://github.com/karimnyumba
- Borwe: https://github.com/Borwe
- Bahara Jr: https://github.com/BaharaJr
- Kdaxh: https://github.com/kdaxh
- Lupyana: https://github.com/lupyana
- Farajael: https://github.com/farajael
- Gabriel Dee: https://github.com/Gabriel-Dee
- Gecko: https://github.com/gekkowrld
- Isacka James: https://github.com/isaka-james

::right::
- Neicore: https://github.com/neicore
- Lary Mak: https://github.com/larymak
- BM Steven: https://github.com/bmsteven
- Nyagawa: https://github.com/Njoxpy
- Isaya: https://github.com/isayaexavery
- Alpha Olomi: https://github.com/alphaolomi
- Fredy German: https://github.com/fredygerman
- Emma: https://github.com/emma255
- Genie: https://github.com/genie360s
- Ringo: https://github.com/ringoebenezer
- Louq: https://github.com/Louq-Tech

---
transition: none
layout: center
class: text-center
---

## Thank you!

Github: @AvicennaJr <br>
Twitter: @AviTheDev <br>
Email: fuad@subcode.africa <br>

# alneuma

Software developer focused on systems and kernel-level C.
Currently completing the program at [42 Berlin](https://42berlin.de/), a peer-reviewed, project-only curriculum without teachers but a lot of self-directed learning.

![C](https://img.shields.io/badge/C-5C6D7E?style=flat-square&logo=c&logoColor=A8B9CC) ![C++](https://img.shields.io/badge/C++-5C6D7E?style=flat-square&logo=cplusplus&logoColor=A8B9CC) ![Linux](https://img.shields.io/badge/Linux-2C6BED?style=flat-square&logo=linux&logoColor=white)

**Open to junior roles in systems, embedded or backend with C or C++ · based in Berlin, available immediately for full-time positions**

## Languages

German (native) · English (fluent) · French, Spanish, Chinese (basic)

## Projects

### [FWL - FIFO Word Logger](https://github.com/alneuma/fwl_kernel_module)

![C](https://img.shields.io/badge/C-5C6D7E?style=flat-square&logo=c&logoColor=A8B9CC) ![Linux](https://img.shields.io/badge/Linux-2C6BED?style=flat-square&logo=linux&logoColor=white) ![kernel](https://img.shields.io/badge/-kernel-6B6B6B?style=flat-square) ![character device](https://img.shields.io/badge/-memory%20accounting-6B6B6B?style=flat-square) ![concurrency](https://img.shields.io/badge/-concurrency-6B6B6B?style=flat-square) ![transactional state mutation](https://img.shields.io/badge/-transactional%20state%20mutation-6B6B6B?style=flat-square) ![workqueues](https://img.shields.io/badge/-workqueues-6B6B6B?style=flat-square) ![memory accounting](https://img.shields.io/badge/-memory%20accounting-6B6B6B?style=flat-square)

> **What this is:** A loadable kernel module for Linux 6.12.105\
> **Context:** industry-issued exercise\
> **Dev time:** ~2.5 weeks, including environment setup and research\
> **Team size:** solo

What looks deceptively simple at the surface turns into a hog of complexity when taken seriously: write words to a queue, read them back, do some periodic logging. What could possibly go wrong?\
Managing partial failures, transactional state mutations, per-open-file-description state, resource accounting, defining a lock order, timer drift, clarifying under-specified semantics and dealing with asynchronous logging invalidating existing state are all problems that gave me headaches.\
The README walks through every semantics decision, many implementation details, and states plainly what was tested and what wasn't.

### [Webserv](https://github.com/jhelbig42/webserv)

![C++98](https://img.shields.io/badge/C++98-5C6D7E?style=flat-square&logo=cplusplus&logoColor=A8B9CC) ![Linux](https://img.shields.io/badge/Linux-2C6BED?style=flat-square&logo=linux&logoColor=white) ![TCP](https://img.shields.io/badge/TCP-6B6B6B?style=flat-square) ![HTTP](https://img.shields.io/badge/HTTP-6B6B6B?style=flat-square)

> **What this is:** An HTTP server built from scratch. No external libraries, only what the language gives you\
> **Context:** school project\
> **Dev time:** several months\
> **Team size:** 3\
> **Role:** developer

A small functional webserver based on HTTP/1.0.

Features:
- GET, HEAD, POST and DELETE methods
- CGI
- Handling multiple client requests with `poll()` and interleaved serving, remembering request state
- Serving different websites on different interface/port pairs
- Extensive configuration options

My contributions:
- Co-developed the overall architecture
- Template-based multi-level logging system
- A well-documented buffer class as essential infrastructure for other parts of the program
- An expandable, well documented config-parser that emits descriptive error messages
- Most LOC (I know, not a quality)

### [Minishell](https://github.com/alneuma/minishell)

![C99](https://img.shields.io/badge/C99-5C6D7E?style=flat-square&logo=c&logoColor=A8B9CC) ![Linux](https://img.shields.io/badge/Linux-2C6BED?style=flat-square&logo=linux&logoColor=white)

> **What this is:** A small Unix shell: env vars, pipes, redirects, heredoc, globbing, logical operators, built-ins\
> **Context:** school project\
> **Dev time:** several months\
> **Team size:** 2\
> **Role:** project lead

More info here

## How I work

- Writing code is how I organize my thoughts; code matures through iteration.
- Some challenges are still best solved off screen.
- Deep-diving into unfamiliar territory and complex challenges is what I love best.
- After every idea for how to make it work, ask: what could go wrong?
- Almost daily peer code reviews at my school. We all mentor each other.

## AI usage

- locating documentation
- clarifying unfamiliar APIs
- reviewing written code
- probing for failure cases

I don't let AI write the code. Designing an architecture and implementing it myself is the fun part.

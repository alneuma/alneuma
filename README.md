# Alrik Neumann

Software developer focused on systems and kernel-level C.
Enrolled at [42 Berlin](https://42berlin.de/), a peer-reviewed, project-only curriculum without teachers but a lot of self-directed learning.

![C](https://img.shields.io/badge/C-5C6D7E?style=flat-square&logo=c&logoColor=A8B9CC) ![C++](https://img.shields.io/badge/C++-5C6D7E?style=flat-square&logo=cplusplus&logoColor=A8B9CC) ![Linux](https://img.shields.io/badge/Linux-2C6BED?style=flat-square&logo=linux&logoColor=white)

**Open to junior roles in systems, embedded or backend with C or C++ · based in Berlin, available immediately**

## Projects

### [FWL - FIFO Word Logger](https://github.com/alneuma/fwl_kernel_module)

![C](https://img.shields.io/badge/C-5C6D7E?style=flat-square&logo=c&logoColor=A8B9CC) ![Linux](https://img.shields.io/badge/Linux-2C6BED?style=flat-square&logo=linux&logoColor=white) ![kernel](https://img.shields.io/badge/-kernel-6B6B6B?style=flat-square) ![concurrency](https://img.shields.io/badge/-concurrency-6B6B6B?style=flat-square) ![transactional state mutation](https://img.shields.io/badge/-transactional%20state%20mutation-6B6B6B?style=flat-square) ![workqueues](https://img.shields.io/badge/-workqueues-6B6B6B?style=flat-square) ![memory accounting](https://img.shields.io/badge/-memory%20accounting-6B6B6B?style=flat-square)

> **What this is:** A dynamically loadable character device for Linux kernel 6.12.105\
> **Context:** industry-issued exercise\
> **Dev time:** ~2.5 weeks, including environment setup and research\
> **Team size:** solo

What looks deceptively simple at the surface turns into a hog of complexity when taken seriously: write words to a queue, read them back, do some periodic logging. What could possibly go wrong?\
Managing partial failures, transactional state mutations, per-OFD state, resource accounting, defining a lock order, timer drift, clarifying under-specified semantics and dealing with asynchronous logging invalidating existing state are all problems that gave me headaches.\
The README walks through every semantics decision, many implementation details, and states plainly what was tested and what wasn't.

### [Webserv](https://github.com/alneuma/webserv)

![C++98](https://img.shields.io/badge/C++98-5C6D7E?style=flat-square&logo=cplusplus&logoColor=A8B9CC) ![Linux](https://img.shields.io/badge/Linux-2C6BED?style=flat-square&logo=linux&logoColor=white) ![TCP](https://img.shields.io/badge/TCP-6B6B6B?style=flat-square) ![HTTP](https://img.shields.io/badge/HTTP-6B6B6B?style=flat-square)

> **What this is:** An HTTP/1.0 server written from scratch. No external libraries, only what the language gives you\
> **Context:** school project\
> **Dev time:** several months\
> **Team size:** 3\
> **Role:** developer

Concurrent client handling, GET/HEAD/POST/DELETE, CGI. Mine: the abstraction
barrier between the network interface and the HTTP module, and an extensible
config-file parser.

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

## Languages

German (native) · English (fluent) · French, Spanish, Chinese (basic)

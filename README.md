<h1 align="center">
    uman
  <br>
</h1>

<h4 align="center">A command-line utility for performing reverse DNS lookups</h4>

<p align="center">
  <a href="#install">🏗️ Install</a> •
  <a href="#usage">⛏️ Usage</a> •
  <a href="#contribute">🤝 Contribute</a>
  <br>
</p>

---

## Install

To install uman, run the following command:

```sh
go install github.com/tal7aouy/uman/cmd/uman@v1.0.0
```

## Usage

This utility allows you to perform reverse DNS lookups on IP addresses. Here are some examples of how to use the tool:

- **Look up a single IP address:**

  ```sh
  uman -i "domain.com"
  ```

- **Look up a list of IP addresses from a file:**

  ```sh
  uman -l host_list.txt
  ```

- **Pipe input from another command:**

  ```sh
  echo "domain.com" | uman
  ```

  ```sh
  cat host_list.txt | uman
  ```

### Available Command-Line Flags

| Flag | Description                                                            | Example                 |
| ---- | ---------------------------------------------------------------------- | ----------------------- |
| `-i` | Specify a single target IP address for reverse DNS lookup.             | `uman -i domain.com`    |
| `-l` | Provide the path to a file containing a list of IP addresses.          | `uman -l host_list.txt` |
| `-c` | Set the level of concurrency for concurrent DNS lookups (default: 10). | `uman -c 20`            |
| `-r` | Specify resolvers for reverse DNS lookup.                              | `uman -r domain.com`    |
|      | You can provide a single IP address or a path to a file.               | `uman -r resolvers.txt` |

## Contribute

We welcome contributions to **uman**! If you're looking to help, please consider the following:

- **Fork and Clone**: Start by forking the repo and then cloning it locally.
- **Pick an Issue**: Look through the open issues. If you're new, look for ones tagged as "good first issue."
- **Feature Suggestions**: Have an idea for a new feature? File an issue discussing your idea openly, so it can be collaborated on.
- **Pull Requests**: After making your changes in a new branch, send a pull request. Make sure your code adheres to the existing style of the project to increase the chance of your pull request being accepted.
- **Code Review**: Be open to receive feedback and participate in discussions on your pull request.

Looking forward to your contributions!

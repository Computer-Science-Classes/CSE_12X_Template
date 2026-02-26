# UW Seattle CSE 12X CI Template

## Usage

Make sure you have "make" installed to your PATH.

Use

```bash
make run module=<module name>
```

To run a project.

Example

```bash
make run module=c99-example-project
```

## Adding a new project

Make a new directory per project with internal structure src/main/java.
Place a pom.xml at root of the new directory and copy and paste the pom.xml
from c99-example-project and change `artifactId` and `mainClass` only.

Note: `mainClass` points to the file which contains the java main class.

## Setup Pre-commit

Setup pre-commit hook

```bash
ln -s ../../scripts/pre-commit.sh .git/hooks/pre-commit
chmod +x scripts/pre-commit.sh
```

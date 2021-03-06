# nebula-go

**IMPORTANT: Code of Nebula go client has been transferred from [nebula-clients](https://github.com/vesoft-inc/nebula-clients) to this repository(nebula-go), and new releases in the future will be published in this repository.
Please update your go.mod and imports correspondingly.**

Official Nebula Go client which communicates with the server using [fbthrift](https://github.com/facebook/fbthrift/). Currently the latest stable release is **[v2.0.0-ga](https://github.com/vesoft-inc/nebula-go/tree/release-v2.0.0-ga)**

The code in **master branch** will be updated to accommodate the nightly changes made in Nebula Graph.
To Use the console with a stable release of Nebula Graph, please check the branches and use the corresponding version.

| Client version | Nebula Service Version|
|:--------------:|:-------------------:|
|   **[v1.0.0](https://github.com/vesoft-inc/nebula-go/tree/v1.0)**              |       1.x.x         |
|   **[v2.0.0-ga](https://github.com/vesoft-inc/nebula-go/tree/v2.0.0-ga)**      |       2.0.0-ga, 2.0.1    |
|   **[v2.0.0-master](https://github.com/vesoft-inc/nebula-go/tree/master)**     |       2.0.0-nightly |


Please be careful not to modify the files in the nebula directory, these codes were all generated by fbthrift.

## Install & Update

```shell
// For 2.x version
$ go get -u -v github.com/vesoft-inc/nebula-go/v2@master

// For 1.x version
$ go get -u -v github.com/vesoft-inc/nebula-go/@master
```
You can specify the version of Nebula-go by substituting `<tag>` in `$ go get -u -v github.com/vesoft-inc/nebula-go@<tag>`.
For example: `$ go get -u -v github.com/vesoft-inc/nebula-go/v2@v2.0.0-ga`

**Note**: You will get a message like this if you don't specify a tag:
> ```
> $ go get -u -v github.com/vesoft-inc/nebula-go/v2@master
> go: github.com/vesoft-inc/nebula-go/v2 master => v2.0.0-20210506025434-97d4168c5c4d
> ```
> Here the ` 20210506025434-97d4168c5c4d` is a version tag auto-generated by Github using commit date and SHA.
> This should match the latest commit in the master branch.

## Usage example

[Simple Code Example](https://github.com/vesoft-inc/nebula-go/tree/master/basic_example/graph_client_basic_example.go)

[Code Example with Gorountines](https://github.com/vesoft-inc/nebula-go/tree/master/gorountines_example/graph_client_goroutines_example.go)



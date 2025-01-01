# Java Lab 16 (Task 1)
This is an introduction to the Spring Boot framework and part of the Java development course at the Vistula University. The repository contains a simple web application which greets the user visiting the `/greeting` page.


## Getting started

### Prerequisites
- OpenJDK 21
- Maven
---

From the repository root:

1. Install dependencies and compile.
```sh
mvn install
```

2. Run the web server.
```sh
java -jar target/first-project-java-spring-0.0.1-SNAPSHOT.jar
```

3. Visit `http://localhost:8080` on your browser.

## Routes

<details>
 <summary><code>GET</code> <code><b>/</b></code> A static generic hello Vistula page.</summary>

##### Parameters

> None

##### Responses

> | http code     | content-type                      | response body |
> |---------------|-----------------------------------|---------------|
> | `200`         | `text/html;charset=UTF-8`         | HTML page     |

</details>

<details>
 <summary><code>GET</code> <code><b>/greeting</b></code> A dynamic greeting page with a photo.</summary>

##### Parameters

> | name              |  type  | data type | description                    |
> |-------------------|--------|-----------|--------------------------------|
> | `name`            |  query | string    | The name of the user to greet. |

##### Responses

> | http code     | content-type                      | response body |
> |---------------|-----------------------------------|---------------|
> | `200`         | `text/html;charset=UTF-8`         | HTML page     |

</details>

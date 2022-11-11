# GO API CRUD
A simple crud API written with Go.

### How to install
```sh
git clone git@github.com:code-pisces/go-simple-crud-api.git

go install

go run main.go
```

## API routes

<b>METHOD GET</b> <br/>
<b>ENDPOINT:</b> /movies <br/>
<b>GET ALL</b> <br/>

```bash
# RESPONSE:
[
	{
		"id": "1",
		"Isbn": "438227",
		"title": "Movie One",
		"director": {
			"firstname": "John",
			"lastname": "Doe"
		}
	},
	{
		"id": "2",
		"Isbn": "45455",
		"title": "Movie Two",
		"director": {
			"firstname": "Steve",
			"lastname": "Smith"
		}
	},
	{
		"id": "727887",
		"Isbn": "438256",
		"title": "Movie Trhee",
		"director": {
			"firstname": "Choco",
			"lastname": "Carneiro"
		}
	}
]
```


<b>METHOD GET</b> <br/>
<b>ENDPOINT:</b> /movies/:id <br/>
<b>GET BY ID</b> <br/>

```bash
# RESPONSE:
{
	"id": "1",
	"Isbn": "438227",
	"title": "Movie One",
	"director": {
		"firstname": "John",
		"lastname": "Doe"
	}
}
```

<b>METHOD POST</b> <br/>
<b>ENDPOINT:</b> /movies <br/>
<b>CREATE</b> <br/>

```bash
# REQUEST
{
	"Isbn": "438256",
	"title": "Movie Trhee",
	"director": {
		"firstname": "Choco",
		"lastname": "Carneiro"
	}
}

# RESPONSE:
{
	"id": "727887",
	"Isbn": "438256",
	"title": "Movie Trhee",
	"director": {
		"firstname": "Choco",
		"lastname": "Carneiro"
	}
}
```


<b>METHOD PUT</b> <br/>
<b>ENDPOINT:</b> /movies/:id <br/>
<b>UPDATE</b> <br/>

```bash
# REQUEST
{
	"Isbn": "438256",
	"title": "Movie Trhee",
	"director": {
		"firstname": "Choco",
		"lastname": "O Carneiro"
	}
}

# RESPONSE:
{
	"id": "727887",
	"Isbn": "438256",
	"title": "Movie Trhee",
	"director": {
		"firstname": "Choco",
		"lastname": "O Carneiro"
	}
}
```


<b>METHOD DELETE</b> <br/>
<b>ENDPOINT:</b> /movies/:id <br/>
<b>DELETE BY ID</b> <br/>

```bash
# RESPONSE:
[
	{
		"id": "1",
		"Isbn": "438227",
		"title": "Movie One",
		"director": {
			"firstname": "John",
			"lastname": "Doe"
		}
	},
	{
		"id": "2",
		"Isbn": "45455",
		"title": "Movie Two",
		"director": {
			"firstname": "Steve",
			"lastname": "Smith"
		}
	},
	{
		"id": "727887",
		"Isbn": "438256",
		"title": "Movie Trhee",
		"director": {
			"firstname": "Choco",
			"lastname": "Carneiro"
		}
	}
]
```

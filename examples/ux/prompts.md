---
runme:
  id: 01JC6WY5QG3VZ9W2HRY1CKZ1D3
  version: v3
---

## Prompt configuration

Configure how you want users to be prompted for input.

**With a placeholder:**

```sh {"id":"01JC6WZCERVJZRQJ0BZJRMKME6","name":"placeholder-prompt"}
export FAVORITE_FOOD=[Enter food name here..]
echo "My favorite food is: $FAVORITE_FOOD"
```

**With a default:**

```sh {"id":"01JC6X47FCSYAAD907NPQ4PKAS","name":"default-prompt"}
export MY_NAME="Tom from Myspace"
echo "MY_NAME set to $MY_NAME"
```

**Don't ask**: Configured by clicking `configuration`, and setting `promptEnv` to `No`.

```sh {"id":"01JC6X7Z5ARXZX424SBWD419DG","name":"dont-ask-prompt","promptEnv":"no"}
export MY_ENV="dev"
echo "MY_ENV is set to $MY_ENV"
```
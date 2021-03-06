# github-actions-course



### **Branch** dispatch-event [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17389694#overview)
_URL_
```
https://api.github.com/repos/telman-devops/github-actions-course/dispatches
```
_Params with POST request_
```
{
    "event_type":"build",
    "client_payload": {
        "env": "production"
    }
}
```
> Example [Github](https://docs.github.com/en/rest/reference/repos#create-a-repository-dispatch-event)
---
### **Branch** filtering-workflows-by-branches-tags-and-paths [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17392734#overview)

```
on:
  push:
    branches:
      - master
      - "feature/**" # matches featur/featA, feature/featB, doesn't match feature/feat/a
      - "!feature/featc"
    tags: 
      - v1.*
    paths: 
      - "**.js"
      - "!filename.js"
    # paths-ignore:
    # - 'docs/**'
```

> Example [Github](https://docs.github.com/en/rest/reference/repos#create-a-repository-dispatch-event)

---
### **Branch** default-and-custom-environment-variables [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17438370#overview)

Add new file `env.yml`

> Example [Github](https://docs.github.com/en/actions/reference/environment-variables)

---
### **Branch** encrypting-environment-variables [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17439746#overview)

```
secrets.GITHUB_TOKEN
```

---
### **Branch** using-the-github-token-secret-for-authentication [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17447354#overview)

* Push a random file
* Create issue using REST API

> Example [Github](https://docs.github.com/en/actions/reference/authentication-in-a-workflow)

---
### **Branch** encrypting-and-decrypting-files [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17450244#overview)

* create secret file secret.json.gpg, use [GPG](https://www.gnupg.org/)
* add job decrypt in `env.yml`

> Example [Github](https://docs.github.com/en/actions/reference/encrypted-secrets)

---
### **Branch** expressions-and-contexts [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17452726#overview)

* create `context.yml` file

> Example [Github](https://docs.github.com/en/actions/reference/context-and-expression-syntax-for-github-actions)

---
### **Branch** using-functions-in-expressions [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17458564#overview)

* add job **functions** in `context.yml`

> Example [Github](https://docs.github.com/en/actions/reference/context-and-expression-syntax-for-github-actions#functions)

---
### **Branch** the-if-key-and-job-status-check-functions [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17458614#overview)

* the **if** key in _job_ and _step_ places

> Example [Github](https://docs.github.com/en/actions/reference/context-and-expression-syntax-for-github-actions#job-status-check-functions)

---
### **Branch** using-the-setup-node-action [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17584154#overview)

* For example, we change Node version in container

> Example [setup-node](https://github.com/actions/setup-node)


---
### **Branch** creating-a-matrix-for-running-a-job-with-different-environments [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17584562#overview)

* Add strategy in our job, and use array

---
### **Branch** including-and-excluding-matrix-configurations [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17586302#overview)

* Implement _include_ and _exclude_ in **strategy** 

---
### **Branch** using-docker-containers-in-jobs [Udemy lesson](https://www.udemy.com/course/github-actions/learn/lecture/17588620#overview)

* create new workflow `container.yml`

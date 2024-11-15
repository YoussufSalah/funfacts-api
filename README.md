# Funfacts API

## How to use:

1.  **Clone The Repo:**
    -   Run in your terminal:
        ```bash
          git clone https://github.com/YoussufSalah/funfacts-api.git
        ```
2.  **Adding Environment Variable:**
    -   Add the `USER_SITE` and `PORT` variables in a .env file (explained below).
3.  **Running The API Locally:**
    -   Run `cd funfacts-api`.
    -   Run `node index.js`, and we're done!

Now you're ready to make requests to the API!

## Environment Variables:

-   `USER_SITE` : Set this to the URL of your website that will fetch the API.
-   `PORT` : Define the server port (default is `3000`).

## Routes:

-   `/api/fact` **- Returns a random fact.**

    -   **Example** Response:

        ```json
        // http://localhost:3000/api/fact

        {
            "status": "success",
            "data": {
                "randomFunfact": {
                    "text": "A human could swim through a blue whale's veins.",
                    "category": "animals"
                }
            }
        }
        ```

-   `/api/fact?category={category_name}` **- Returns a random fact within a specific category.**

    -   **Example:** `http://localhost:3000/api/fact?category=animals`
    -   **Available Categories:** food, science, animals, history, space, inventions, engineering, geography, literature, human body, language, health, society, weather, money.
    -   **Example Response:**

        ```json
        // http://localhost:3000/api/fact?category=animals

        {
            "status": "success",
            "data": {
                "randomFact": {
                    "text": "A human could swim through a blue whale's veins.",
                    "category": "animals"
                }
            }
        }
        ```

---

### Wanna support me ?

[Buy me a coffee!](https://ko-fi.com/youssufsalah)

---

#### Tags:

#javascript #js #node #nodejs #node_js #node-js #node.js #api #REST #rest #RESTFUL #restful #funfact_generator #funfactgenerator #random #random_generator #randomgenerator #funfact #funfactapi #funfact_api

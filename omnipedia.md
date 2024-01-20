# Website for Omnipedia

Repo: https://github.com/Omnipedia/RC-Hackathon-Website

Full disclosure, we have a draft for this we're happy with and as this would be the marketing website for us, it's more about graphics than functionality. Our 'marketing team' is pretty happy with our current site, it's just missing images. I think that as a hackathon, you'd get more out of the Chat UI. 

That said, if you want to go this route, we need a few pages. 
1. The main page showing two things. A a grpahic showing the basic premise (Wikipedia/PubMed/ArXiv/<< Your data here >>  -> A black box representation of our product -> A question and a text document answering it with citations from the input documents) an automated demo of the product (for which you may use the Postman collection I will provide). It does need to have taglines and such. Think OpenAI's page. They've got a variety of "We're here to save humanity from the evil robots" all over their site.
2. There needs to be a form page to contact us. The user would input their email address and a short message, say, 2000 characters.

# Chat UI for Omnipedia

Repo: https://github.com/Omnipedia/RC-Hackathon-ChatUI

## Mock API Service
This contains a Mock API Service under `chat-api-mock`. While it is running at [http://0.0.0.0:5001](http://0.0.0.0:5001), you may find the api ReDoc documentation and example api calls at [http://0.0.0.0:5001/api-doc](http://0.0.0.0:5001/api-doc). An error will trigger under the following conditions:
1. The last user message is simply 'error'
2. There are no messages in the conversation.
3. The last message belongs to the Assistant
### Valid API Call
```bash
curl --location 'http://0.0.0.0:5001/streaming_conversation' \
--header 'Content-Type: application/json' \
--header 'Connection: keep-alive' \
--header 'Cache-Control: no-cache' \
--data '[
  {
    "User": "String"
  }
]'
```
### Trigger Mock API Error
```bash
curl --location 'http://0.0.0.0:5001/streaming_conversation' \
--header 'Content-Type: application/json' \
--header 'Connection: keep-alive' \
--header 'Cache-Control: no-cache' \
--data '[
  {
    "User": "error"
  }
]'
```

## Acceptance Criteria
- Given I enter a query, when the response is returned, then it contains the citation, and a reference to the source text appears on the right.
- Given the reference is printed, when I click the expand button next to it, then I see the original source passage.
- Given the reference is printed, when I click the reference, then I am taken to the original source.
- Given the response is returned, when I look at the source text, it is a passage or table that stands on it's own.
- Given the response is returned, when the response prints a cited piece of text, the reference and source appear in a column on the right.
- Given the response is returned, when the citations are printed, the references follow the preferred citation format.
- Given the response is returned, when the citations are printed, the citations are are numbers in square brackets, and the matching reference has the same number.
- Given the response is returned, when the citations and references are printed, the citations and references are numbered contiguously starting from 1.
- Given the product demo returns a response with sources, when the user clicks on the citation, then they are navigated to the source text.
- Given the machine returns a response, when it produces the citation in the text, only reference associate with the citations are shown in the sidebar.

## Discussion

> Me: You wanted to have a website for your company, right? Can you prepare a repo or repos for it, please?
>
> Michael McCulloch: Oh for sure.
>
> Me: I personally prefer monorepos due to ease of source control and ease of writing code elated to CI/CD.
>
> Michael McCulloch: So, what were you thinking you wanted to build?
>
> Michael McCulloch: Giving you repo access to our repo would require NDAs all around, which seems a bit heavy handed. Would a separate repo for the UI be acceptable?
>
> Me: Either actix or axum  backend and literally whatever for the frontend.
>
> Michael McCulloch: Ah got you.
>
> Me: "Would a separate repo for the UI be acceptable?". Totally!
>
> Michael McCulloch: I would also be willing to prepare a mock API binary for you to test against alternatively, i can provide the api signature snippets and you can build the binary, alternatively I can privide a screenshot of the OpenAPI documentation and you can build something into PostMan.
>
> Micheal McCulloch: And, would you like to build the marketing website, or the chat interface?
>
> Me: That's a question for everyone who would be interested!
>
> Me: I'll need to start my day now. I'll check the Discord later!
>
> Michael McCulloch: Ok, well the marketing website is detached from everything so no api is currently needed. We're using a tool (WebStudio) to build it and it's in a draft state.
>
> Michael McCulloch: The chat UI however would require API Access. I know I would prefer if the hackathon was around the Chat UI, but like you said: "That's a question for everyone who would be interested!".
>
> Michael McCulloch: "build something into PostMan". I will prepare a Postman collection for you today, then you can do as you wish. Let me know what the group decides.

## Dialguide: Aligning Dialogue Model Behavior with Developer Guidelines


Dialogue models have the ability to generate coherent and fluent responses, but controlling their behavior can be challenging, as they may produce non-engaging or unsafe outputs. This unpredictability undermines user trust and limits their real-world utility. To tackle this issue, we present DIALGUIDE, a novel framework that enables control over dialogue model behavior through natural language rules, referred to as guidelines. These guidelines specify the applicable context and the desired content of the response, aligning the models more closely with developer expectations and intentions. We evaluate DIALGUIDE on three tasks related to open-domain dialogue response generation: guideline selection, response generation, and response entailment verification. Our dataset consists of 10,737 positive and 15,467 negative dialogue context-response-guideline triplets spanning two domains: chit-chat and safety. Baseline models are provided for each task, and their performance is benchmarked. The results demonstrate that DIALGUIDE effectively produces safe and engaging responses that adhere to developer guidelines.

<img src="/figures/dialguide-teaser.png" width="200" height="600">


## Dataset description

We provide train, test and validation files for the following datasets:

- dialguide-BST-{split} - contains context-guidelines-response for Dialguide-safety dataset. response-type indicates whether response entails or refutes the guideline+context
- dialguide-safety-{split} - contains context-guidelines-response for Dialguide-safety dataset
- guidelineretrieval-bst{split} - The dataset contains instances with the following attributes:
    - "context": A list of sentences representing the conversation context.
    - "guideline_written": Gold written guideline for the conversation.
    - "gtguideline_condition": Gold condition associated with the guideline.
    - "positive_ctxs": A list of positive guidelines realted to the context, with each example having a "title" and "text".
    - "hard_negative_ctxs": A list of hard negative guidelines, with each example having a "title" and "text".
    
## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the CC-BY-NC-4.0 License.


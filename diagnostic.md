# Ember Components Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  Give an example of a visual hierarchy that could be modeled with components.

    ```md
    A list of lists.
    ```

1.  What is the command to generate a new component called '`my-map`'?

    ```sh
    ember g componenet my-map
    ```

1.  What files are edited to produce a component, and what are their
    responsibilities?

    ```md
    a component directory is created containing 'my-map' inside which is a component.js file as well as a template.hbs
    ```

1.  Suppose you have a component '`my-contact`', which is loaded from
    '`app/contacts/template.hbs`' when visiting the `/contacts` path. What is
    the syntax for loading this component inside that template?

    ```html
    {{#each model as |contact|}}
    {{/each}}
    ```

    Each contact has multiple phone numbers. Suppose you also have '`my-phone`'
    nested under '`my-contact`'. What is the code you would write in
    '`app/components/my-contact/template.hbs`' to load the nested component and
    pass it data?

    ```html
    {{my-contact.my-phone}}
    ```

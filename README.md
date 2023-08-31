
<h1 align="center">Only Prompt vs Prompt with Context<hi>

 

 

### Glossary 


   - Introduction 

   - Komadaz App     

   - Only Prompt

        - Prompt Template

        - Models

            -  GPT 3.5 

                - Chat Flow

                - Results

            -  GPT 4 

                - Chat Flow

                - Results    

     - Prompt with Context

        - Prompt Template

        - Context Template

        - Models

            -  GPT 3.5 

                - Chat Flow

                - Results

            -  GPT 4 

                - Chat Flow

                - Results    


     - Conclusion

        - Models 

        - Language

        - When to Use Only Prompt? (Opinion)

        - When to Use Context? (Opinion)


 

---

 

#### Introduction 

     This report is to a discussion about best Practices

     about using Prompt and Context with LLMs and insights 

     about Comparison Data that Should to use in these cases

     depending on [Komadaz App]() and [Bindwood]() that is the app used to test 

     results on this report.


 

---

- **Only Prompt** <br>

    A prompt is a concise instruction or query provided to

    a language model to generate desired responses.


    - Prompt Template In Arabic 

        You Can Find Prompt [here]() the Prompt 

        was written in Arabic to give the model best

        practice as the language of

        intended users and is Arabic like provided data


    -  Models 

        The models used to test this use case is 

        (Gpt 3.5-turbo & Gpt 4) 


        - Gpt 3.5-turpo :

              - Chat Flow

            - You can find chat flow  with Arabic [here]().

            - You can find chat flow  with English [here]().

              - Results

                        -Language

              - when using this models the results 

              i think is very good but the total number

              of tokens for this model is 4096 and when 

              using Arabic Prompt template the number of

              tokens is very tall comparing the results 

              of Yasser when using English Prompt template

              and for that i can't provide the prompt with all details

              because of the limitation on context window size.

 

 

        - Gpt 4 -8k version:

              - Chat Flow

            - You can find chat flow  with Arabic [here]().

            - You can find chat flow  with English [here]().

              - Results

                        -Language

              - when using this models the results 

              i think is wasn't different comparing to 

              GPT 3.5 as 2 models acts well, 

                          but the total number of tokens for this model is 8000 

              and when using this model can accept the Arabic Prompt

              template with all details i want to provide in Prompt

 

 

    - Prompt Template In English 

        You Can Find Prompt [here]() the Prompt 

        was written in English because the models 

        are trained more in English language and they 

        can understand the Prompt well and can make a better reponses 

        from understanding the prompt.

 

    -  Models 

        The models used to test this use case is 

        (Gpt 3.5-turbo & Gpt 4) 


        - Gpt 3.5-turpo :

              - Chat Flow

            - You can find chat flow  with Arabic [here]().

            - You can find chat flow  with English [here]().

              - Results

                        -Language

             -  with this model i use prompt with length 12000 char

                in prompt template and GPT3 gave us a good result.



 

 

        - Gpt 4 -8k version:

              - Chat Flow

            - You can find chat flow  with Arabic [here]().

            - You can find chat flow  with English [here]().

              - Results

                        -Language

                - This Model generaate a better results but 

                  in this case i didn't see a huge difference 

                  for that if we need to reduce expnses i recommend

                  to use GPT 3.5 turbo.

 

 

 

---

 

-  **Prompt with Context** <br>

    Prompt with Context involves providing both a prompt and additional context

    or examples to enhance the language model's understanding and performance.


 

    - Prompt Template IN ARABIC

        - You Can Find Prompt [here]() the Prompt 

        was written in Arabic to give the model best

        practice as the language of

        intended users and is Arabic like provided data.

    - Context Template

        - You Can Find Context [here]().



    -  Models 

        The models used to test this use case is 

        (Gpt 3.5-turbo & Gpt 4) 


        - Gpt 3.5-turpo :

              - Chat Flow

            - You can find chat flow  with Arabic [here]().

            - You can find chat flow  with English [here]().

              - Results

                        -Language

              - After using a prompt of 5k char and 12k char in the context 

               with splitting each section in the context in a seprate paragraphes

               we got a better results but i see in this case that we can use prompt only.

 

 

    - Prompt Template IN ENGLISH

        - You Can Find Prompt [here]() the Prompt 

        was written in Arabic to give the model best

        practice as the language of

        intended users and is Arabic like provided data.

    - Context Template

        - You Can Find Context [here]().



    -  Models 

        The models used to test this use case is 

        (Gpt 3.5-turbo & Gpt 4) 


        - Gpt 3.5-turpo :

              - Chat Flow

            - You can find chat flow  with Arabic [here]().

            - You can find chat flow  with English [here]().

              - Results

                        -Language

              - when using this models the is very detailed answer 

                and provide me to use short prompt with Arabic language, 

                but i think for this use case if we used the prompt template 

                with English tokens to handle the size of context window it's

                better practice.



 

 

        - Gpt 4 -8k version:

            For me I can't test context on this version because of credentials 

            but i think it is not necessary.

 

 

 

 

---

 

-  **Conclusion** <br>

     
    - Models For me I didn't  find a huge difference in performance between Models when responding

      and the both of Models act well and the influenced difference is limitation of window size.

    - English Prompt is better than Arabic Prompt as the Arabic is require more tokens size.

    - When to Use Only Prompt? (Opinion)

      It's a critical as it is depending on many factors (language,model,..eg)

      but depending on what i said i this report and my experience with Komandaz

      * We can use only prompt the we have maximum 10 main leafs in our [Scenario]

        as every main point  question can contain many sub questions for tha to make prompt 

        have all details i think 10 main points for GPT 3.5-turbo and we can extreme this 

        number for GPT 4-8k  to 15.


    - When to Use Context with Prompt?

      Back to Previous answer we can use context when we have more 

      than 10 questions in Gpt3.5 -turpo, more that 15 main leafs in Gpt 4 -8k.


 

      



 

 

---------------------------------------------------------------------

 

- Insights 

    Untill now we see that we have 2 factors (Complexity of Conversation, length of Prompt) 


    - Length Of Prompt depending on which language for example ( in  GPT3 it accepted 12k char of English Prompt

      but didn't accept 9k from arabic Prompt but in GPT4 it accepted both)

 

---

   - Compexity 

        - if we have a not simple structure and sipmle data in this case we can use the prompt only if the prompt 

          will not exeed the allowed number of tokens of our model.

           ![](https://firebasestorage.googleapis.com/v0/b/menialwyschool.appspot.com/o/6.png?alt=media&token=288120a3-0465-4615-ad1b-ee58e00ea783)

        - if our data is complex but with a  simple structure in this case we will use Prompt with context.

            ![](https://firebasestorage.googleapis.com/v0/b/menialwyschool.appspot.com/o/5.png?alt=media&token=cf1f259e-3afd-4df9-95f0-51ee71c232ba)

        - if our simple data  and complex structure we will use only prompt. 

            ![](https://firebasestorage.googleapis.com/v0/b/menialwyschool.appspot.com/o/4.png?alt=media&token=d920fb4e-318c-48cc-b48e-e7414a5c515d)

        - if our data huge and strucutre complex we will use Prompt with Context.

             ![](https://firebasestorage.googleapis.com/v0/b/menialwyschool.appspot.com/o/2.png?alt=media&token=792b8f8e-cf29-4bc2-b525-c456e253fab0)


---

  The best results we will get Prompt with Context but it will be more cost and more time     

 

        and choosing the model will depend also on size of data and the cost needed

 

        as in some cases we can use GPT3 but GPT4 will give a better results 

        but GPT3 is still suitable   

 

----

Why to use a AI Bot? <br>

**our new chat bot have the ability without wasting customer time.**

![](https://firebasestorage.googleapis.com/v0/b/menialwyschool.appspot.com/o/10.png?alt=media&token=29670535-3263-4739-8d62-da65defe33c6)

 

 

![](https://firebasestorage.googleapis.com/v0/b/menialwyschool.appspot.com/o/11.png?alt=media&token=799a334a-f38f-4691-a705-4a1ccf14bb7d)

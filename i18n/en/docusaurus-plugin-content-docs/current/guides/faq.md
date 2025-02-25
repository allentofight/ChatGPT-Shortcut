# FAQs

## Why are the suggested words in English?

AiShort was created to facilitate the use of ChatGPT by non-native English speakers. However, all the suggested words are in English. This is because ChatGPT has a better understanding of English compared to other languages. Even MOSS, the first large-scale Chinese dialogue language model, acknowledges that its English responses are superior to Chinese. Therefore, it is recommended to use English suggested words. (MOSS is no longer available)

Although using non-English suggested words may yield decent results, the outcomes can vary significantly when you input the same non-English prompts again. Since ChatGPT's understanding of non-English prompts varies each time, it is advised to use English prompts for productivity-oriented prompts to ensure the desired output. Furthermore, the responses generated by English prompts are likely to be in English. You can specify the response language as Chinese by adding "respond in Chinese" at the end of the prompt. If your native language is different, please replace "Chinese" with your own native language.

## Do I have to input the prompt every time?

In the API, you can set the prompt as a "system prompt," so you don't need to input the prompt each time. ChatGPT will follow the instructions based on the system prompt.

In the web version of ChatGPT, if you haven't switched the main prompt, you can simply enclose the subsequent reply content in quotation marks, eliminating the need to input the prompt each time. When the generated response does not align with the prompt requirements, it means ChatGPT has forgotten the prompt, and in such cases, you need to re-enter the prompt to reorient it. Additionally, each conversation link is unique, and you can save frequently used conversations as bookmarks for future use.

## Input method search delay

The search function is based on Docusaurus's showcase and has an issue with the input method losing focus on the PC side. After reporting the issue to Docusaurus, they mentioned they would try to fix it, but so far, the problem remains unresolved, with the comment, "FWIW, you should not be using Chinese anyway, since the showcase is not localized." Therefore, I have categorized the search component into two types: mobile and PC. The search logic for mobile remains unchanged, while for PC browsing with a screen width threshold above 768px, I have introduced the "debounce" function to address the input method problem. However, this introduces two issues on the PC side: non-English input needs to be completed within 800 milliseconds, and the PC search refresh changes from instant to an 800-millisecond delay. If you have a better solution, please provide feedback.

## Outputting false information

Although ChatGPT is very powerful, it is not infallible. Sometimes it may output false information. For example, when I needed to input hundreds of pieces of information into AiShort, I had ChatGPT convert the data into a specified format. However, during the conversion process, I noticed that ChatGPT had inaccurately written some of the information. For instance, a label in the text was "movie critic," but ChatGPT changed it to "film critic." While this may not have any impact in the text itself, it would cause an error when used in code. Therefore, when using ChatGPT, it is essential to review its output.

## Suggested words not working well

All the suggested words are sourced from the Internet and are regularly updated. Although I have tested each suggested word, the actual performance may deviate depending on the specific requirements. If you discover any errors, have creative ideas, or possess good suggested words, please feel free to provide feedback and contribute on the [GitHub page](https://github.com/allentofight/ChatGPT-Shortcut/discussions/11).

If you are summarizing or condensing information, you can use GPT to further refine the original responses, thereby enhancing the accuracy of the answers. Moreover, suggested words not only serve for productivity purposes but also help broaden your thinking, stimulate creativity, consider problems from multiple perspectives, and solve issues that are easily overlooked during the thinking process.

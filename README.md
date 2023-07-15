# promptmap

Prompt injection is a type of security vulnerability that can be exploited to control the behavior of a ChatGPT instance. By injecting malicious prompts into the system, an attacker can force the ChatGPT instance to do unintended actions.

promptmap is a tool that automatically tests prompt injection attacks on ChatGPT instances. It analyzes your system prompts to understand its context and purpose. This understanding is used to generate creative attack prompts tailored for the target. promptmap then starts a ChatGPT instance with the system prompts provided by you and sends attack prompts to it. It can determine whether the prompt injection attack was successful by checking the answer coming from your ChatGPT instance.

```
+-----------+                     +-----------+                        
|           |     Attack 1        |           |       +---------------+
|           | <------------------ |           |       |Successful     |
|           | ------------------> |           |       |Prompts        |
|  Target   |  Sorry, can't do    | Attacker  |       |               |
| ChatGPT   |                     |  ChatGPT  |------>|Attack2        |
|           |     Attack 2        |           |       |               |
|           | <------------------ |           |       |               |
|           | ------------------> |           |       |               |
|           |  Of course, can do  |           |       +---------------+
+-----------+                     +-----------+                        
```



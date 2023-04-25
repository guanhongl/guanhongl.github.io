---
layout: essay
type: essay
title: "HELP! My Question Doesn't Work"
# All dates must be YYYY-MM-DD format!
date: 2020-09-10
published: true
labels:
  - StackOverflow
---

## The Age of Questioning

In an ever developing era of technology, the amount of information and knowledge we possess is rapidly expanding and evolving. With so much new information, it becomes increasingly difficult to retain. No one is omniscient which is why it is necessary to ask others for help. In present times, question asking is an essential skill, especially for software engineers who often specialize in many fields. It’s O.K. to ask for help, but the manner in which you ask matters; there’s smart and stupid ways to ask. 

## Smart vs Dumb

#### Smart Questions

```
Q: What does "Memory allocated at compile time" really mean?

In programming languages like C and C++, people often refer to static and dynamic memory 
allocation. I understand the concept but the phrase "All memory was allocated (reserved) during 
compile time" always confuses me.

Compilation, as I understand it, converts high level C/C++ code to machine language and outputs 
an executable file. How is memory "allocated" in a compiled file ? Isn't memory always allocated in 
the RAM with all the virtual memory management stuff?

Isn't memory allocation by definition a runtime concept?

If I make a 1KB statically allocated variable in my C/C++ code, will that increase the size of the 
executable by the same amount?

This is one of the pages where the phrase is used under the heading "Static allocation"...
```

[Smart questions](https://stackoverflow.com/questions/21350478/what-does-memory-allocated-at-compile-time-really-mean) start with refined subject headers. A well-thought and concise header attracts readers and provides them with the main point of your question. The header here clearly asks about memory allocation at compile time. Next, smart questions should provide background and show proof of individual research. The user opens with background information about static and dynamic memory allocation. They then demonstrate their understanding so far based on what research they’ve done. This also displays their desire to understand and not just for the answer. In return for asking a smart question, the user receives a well-constructed answer: they clearly explain what memory allocation at compile time is and provide detailed examples. 

```
A: Memory allocated at compile-time means the compiler resolves at compile-time where certain 
things will be allocated inside the process memory map.

For example, consider a global array:

int array[100];

The compiler knows at compile-time the size of the array and the size of an int, so it knows the 
entire size of the array at compile-time. Also a global variable has static storage duration by default: 
it is allocated in the static memory area of the process memory space (.data/.bss section). Given 
that information, the compiler decides during compilation in what address of that static 
memory area the array will be...
```

#### Dumb Questions

```
Q: Scanf is not working in C

I am trying to work out why the second scanf is not working for me. Here is the code:

#include <stdio.h>
int main() {
    char n;int p;
    printf("Enter the number: ");
    scanf("%d",&p);
    if(p==1) {
        printf("Enter a character: ");
        scanf("%c",&n);
    }
}

In this program the second scanf("%c",&n) is not working. What am I doing wrong? The output of above program is:

Enter a number: 1
Enter a charter: 

It is coming out of compiler.
```

[Dumb questions](https://stackoverflow.com/questions/34049463/scanf-is-not-working-in-c), however, demonstrate a lack of intelligence. The first thing one may notice is the uninspiring header, "Scanf is not working in C". Vague questions like these leave the reader asking more questions and are often time sinks. The user pastes some lines of code that they expect others to analyze. They provide no other useful information and contribute nothing to the problem-solving process. Also, they lazily exhibit a lack of research as this is a common C question that can easily be Googled. The user clearly desires the answer rather than understanding. As a result, they are given short answers that state the property of scanf(), pulled directly from the manual. 

## Be Smarter Today

As an avid Googler of questions, I now know what constitutes a smart question. When asking a question online, you should strive to become active participants in problem-solving. This includes doing your research and asking concisely. Furthermore, you shouldn’t seek the convenience of an answer. Instead, phrase your question in a way that warrants understanding. Smart questions benefit both you and the reader! For aspiring software engineers like myself, asking smart questions will greatly improve productivity in our work environments. 
# Core Principles for Elder-Friendly and Beginner-Friendly UI

These principles provide the foundation for creating interfaces that are easy for older adults and people new to technology. They will guide all future guidelines in this repository.

First, we'll outline "pain triggers" that older adults and people new to technology experience, then we'll outline the principles that will help us avoid these pain triggers.

## Pain Triggers

1. **Cognitive overload** - The user is overwhelmed by the thinking required to parse or interact with the interface. This could be due to the number of options, the complexity of the interface, the lack of a clear path to the desired action or simply poorly worded text.
2. **Physical exertion** - The user is required to exert too much physical effort to parse or interact with the interface. This could be optical or tactile exertion in the form of small text that is hard to read, small buttons that are easy to miss, or a lack of spacing between elements.
3. **Emotional exertion** - The user is given an unclear or negative feedback when they commit an action. This is sometimes unavoidable as the user may have performed an action that was not what they intended. For example, a user may have accidentally deleted a message or file and the app does not provide a "chicken test" confirmation or a way to recover the data.

> **ℹ️ How to Read These Principles**
>
> Each principle below is presented in a consistent format to make them easy to understand and apply:
>
> -   **A tl;dr version**: A quick summary of the principle.
> -   **Justification**: Why this principle matters.
> -   **General guidelines**: How to put the principle into practice.
> -   **Specific examples**: Good and/or bad implementations to illustrate the point.
>
> _Use these principles as a checklist or reference when designing interfaces for older adults and beginners. They are meant to be practical, actionable, and easy to revisit as you build or review your product._

## Principle 1: Simple - Manage Choice Paralysis (Cognitive overload)

_Limit visible calls to action and progressively reveal complexity._

In simple terms: Make sure users are never overwhelmed by the number of options they have. Occupy the top of their attention span with no more than 1-4 clear call-to-actions. The less important the action, the less prominent it should be.

Many older adults and new technology adopters face confusion and frustration when confronted with too many options simultaneously. Apps should minimize the number of visible interactive elements presented at any given time.

Research by [Harleen (2022)](https://openresearch.ocadu.ca/id/eprint/4732/7/Understanding%20the%20cognitive%20burden%20of%20digital%20interactions%20for%20users%20aged%2060%20and%20older.pdf) and [Vaportzis, E., et al. (2017)](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2017.01687/full) demonstrate that excessive UI options can overwhelm older users, leading to reduced digital engagement, and that simplified UI design significantly eases the adoption curve.

Clearly define a hierarchy of actions: primary actions should be fewest in number and prominently visible, secondary actions less prominent, and tertiary actions hidden until explicitly requested or contextually necessary. Adopt progressive disclosure, introducing complexity only as required.

If your interface demands numerous primary actions visible simultaneously, reconsider the product design by consolidating related features or distributing them across multiple screens or dedicated sub-applications. This prevents cognitive overload and ensures the user experience remains focused, guided, and manageable.

The author, Zaid Hassan, has expanded on this principle in his [blog post](https://tinyurl.com/refactoring-ux-for-elders) with a more detailed explanation and examples.

## Principle 2: Comprehensible - Make It Easy to Understand. (Cognitive overload)

_A user will only dare explore your app if they can understand what it does._

In simple terms: Make sure users can understand the interface and the actions they can take. Use plain language and avoid jargon, icons that are not self-explanatory, and text that is not self-explanatory.

When designing apps, we often fall into the trap of taking "a shared understanding between the designer and customer" for granted. Although it may seem obvious to you, it may not be obvious to the user.

A good way to identify this is by workshopping the app with a group of users who are not familiar with the app, being sure to target users who are not tech-savvy - elders, specifically. The only thing better than putting yourself in the shoes of a user is by talking to them first. Having CTAs with vague labels is a good way to trap users into receiving [negative feedback](#principle-4-recoverable--make-it-easy-to-recover-from-mistakes-negative-feedback).

For example, we often assume that users would know to click on a banner that simply states the number of "points" they have earned if they want to redeem them or simply learn more. This is not always the case. A good way to test this is to ask the user to read the banner and then ask them if they would know what to do next. Another common example is the use of icons, which may not always be self-explanatory.

Specific guidelines and techniques will be discussed in the guidelines document.

## Principle 3: Navigable - Make It Easy to Navigate. (Cognitive overload)

_Guide the user to the desired action._

In simple terms: If a user has opened the app with the intention of performing an action, they should know exactly where they need to go.

A common anecdote is when elder mobile users have to call a younger person if they need help with changing the settings of their phone. The user is not sure where to go, and the app does not provide a clear path to the desired action. The settings app is an example of an intentionally complex app with a lot of bells and whistles.

More recently, both Android and iOS have made the settings app more user-friendly by providing a search bar, linearizing task flows and renaming settings to be more descriptive with simpler language. This is a good example of how even a complex application can make itself more approachable.

However, if the stigma of "complex" is still present in the minds of many users with regards to the Settings app, they often wouldn't even try to explore the app to see if it's any easier to use now. This is why prioritizing ease of use very early on in your product's lifecycle can prevent users from being irreversibly turned away from using your app in the future.

If you're a Product Owner writing a User Story, first ask yourself if the persona would be a power-user or a beginner. Accordingly, take a second look at the "user journey" and see if there are any redundant navigation steps that could be avoided.

## Principle 4: Perceivable – Make Everything Easy to See and Hear. (Physical exertion)

_What's easy to see and hear is also easy to operate._

In simple terms: Make sure users can catch all the information on the screen without straining. Use big, clear text in colors that stand out from the background so that people with weaker eyesight can read effortlessly.

A lot of elderly users have a hard time reading small text, even those with prescription glasses might have a number of other challenges due to cataracts, macular degeneration, and other conditions. They need to be able to read the text on the screen without straining.

For example, use a large font on a high-contrast background (dark text on a light background or vice versa) – this helps everyone, especially those who normally need reading glasses.

Also, give information through multiple senses: don’t rely solely on tiny visual cues or faint sounds. If something important happens (like a message is sent or an error occurs), show a visible alert and maybe play a sound (or a vibration) so it’s noticeable.

Very optionally, make buttons and links look like buttons and links – perhaps underline links and give buttons a distinct color or border. This way, even someone unfamiliar with touchscreens can visually tell what’s clickable. This is not a requirement for all apps as each app has a different brand identity, but it is a good practice to follow.

Essentially, nothing in your app should be “hidden” in plain sight: it should be obvious what things are and what they do at a glance.

For users who can’t read small text or any text at all, consider adding voice or audio support – for instance, a feature to read out notifications or the option to speak commands. The bottom line is to communicate in more than one way (text, visuals, sound) so users don’t miss anything crucial.

For more information, see [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/TR/WCAG21/), which is the standard for web accessibility.

## Principle 5: Recoverable – Make It Easy to Recover from Mistakes. (Emotional exertion)

_A user will only dare explore your app if they won't be punished for making mistakes._

In simple terms: If a user makes a mistake, the app should help them recover without frustration.

It's often said that positive reinforcement is more effective than negative reinforcement. This is true, but it's also true that negative reinforcement can be effective if it's done in a way that is not punitive. Non tech-savvy users are quite prone to performing actions that are not what they intended, therefore, it's critical to assure the user that they can recover from their mistakes.

Always provide an “out” – a clearly visible back or home button on each screen, so if they get confused or took a wrong turn, they can easily start over without panic.

For actions that are easily reversible, provide an undo option. For actions that are irreversible, provide a confirmation step before proceeding.

For example, if a user deletes a message by mistake, the app should provide an undo option. If a user wants to delete a file, the app should provide a confirmation step before proceeding. Even more proactively, the app should provide a "chicken test" confirmation before the user commits an action that can be destructive - a simple confirmation that the user wants to proceed and understands the consequences. This can go a long way in preventing misclicks due to "fat" or shaky fingers.

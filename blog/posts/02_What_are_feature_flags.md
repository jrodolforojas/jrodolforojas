# What are Feature Flags?

Do you know what a feature flag is? Me neither a few minutes ago 😅. For work, I had to use it in my current ticket and I want to share it with you! 🥳

<aside>
📝 Feature flags are a software development concept that allows you to **enable or disable** a feature without modifying the source code or requiring a redeploy

</aside>

Basically, you have a feature but you don’t really know if it will work or break something, it’s when feature flags come in. Its function is to determine the code path that will be executed or not. Yes, like a simple `if/else`.

```js
//We want to render a user form depending on the feature flag
if (featureFlags["new_amazing_form"]) {
  renderNewForm();
} else {
  renderOldForm();
}
```

## What happened in the old times? (not really old times 🤭)

<aside>
🤔 Historically, deploy and release were synonymous because code that was deployed to the production environment was automatically running in production.

</aside>

So if a new feature was broken in production we needed to roll back the entire release 🫠, slowing down the velocity of development teams.

With Feature flags we can change that by uploading new code in a production deploy, but not be executed until we release that 😎. Feature flags can solve problems like:

- Manage the feature lifecycle - Active or deactivate the feature depending on who has access to that.
- Remove the stress and risk around releases - If a feature crashes, change the flag to `false` and will disable it, solving the problem without needing to roll back the entire release with all the features or bug fixes.

## When to use feature flags 🤝🏼

Usually, features could take days, weeks, or months to complete it. Once it is finished, it’s time to send it to the war!🫡 Sorry, production jaja. But we don’t really know if it worked or if it breaks another feature.

![https://media.giphy.com/media/NTur7XlVDUdqM/giphy.gif](https://media.giphy.com/media/NTur7XlVDUdqM/giphy.gif)

With Feature flags you define which code will be executed and which will be ignored.

```js
if (featureFlags["register_transport"]) {
  // <-- false ❌
  <RegisterCarForm />;
} else {
  <RegisterSkateboardForm />; // <-- it will be executed 😉
}
```

In another case, we can use Feature flags to give specific users access to a feature. For example, a beta program, so some users can use this new functionality before everyone. Like an `MVP`

### 🛹 → 🚲 → 🚗

## The idea is not having many ifs around the code

Everything is good, but what happens when this **“new code”** will be the current and the old code are no longer useful? That’s the question you need to take care of when you use Feature flags 😉

<aside>
📌 All this information was investigated in [Feature Flags by LaunchDarkly](https://launchdarkly.com/blog/what-are-feature-flags/#:~:text=Feature%20flags%20are%20a%20software,portions%20of%20code%20are%20executed)

</aside>

Hope it will help you,

Pura Vida! 🇨🇷

[@jrodolforojas](https://www.linkedin.com/in/jrodolforojas/)

<div  align="center">
	<a  href="https://summerofcode.withgoogle.com/projects/#4626086438109184"><img  src="https://rocket.chat/wp-content/uploads/2021/02/Frame.png.webp"  width="650"  alt="google-summer-of-code"></a>
	<br>
	<b>
		<p>
		Introduces SpeechToText capabilities into Rocket.Chat as a standalone Rocket.Chat App
		</p>
	</b>
</div>

This summer, I was pleased to get selected for Google Summer of Code'21 under the organization [Rocket.Chat](https://github.com/RocketChat). Working under the organization, my project was to **Introduce SpeechToText capabilities into Rocket.Chat as a standalone Rocket.Chat App**.


## 📙 Abstract

[Rocket.Chat](https://www.npmjs.com/package/react-native-elements) is a modern team chat and collaborating platform written in full-stack JavaScript offering a full featured rich team chat experience on modern browsers, comparable to Slack and Microsoft Teams. Mobile and desktop clients run on iOS, Android, MacOSX, Windows, and Linux. It is one of the largest active open source (permissive MIT source license) nodeJS communications platform communities on GitHub with more than 12Million users worldwide.


Rocket.Chat users have an option of sending audio files or live audio messages to a room or a chat. My project introduces a new native Rocket.chat app that utilises the capabilities of [Rocket.Chat.Apps-Engine](https://github.com/RocketChat/Rocket.Chat.Apps-engine) and allows the user to be able to not only transcribe the audio files but also save the transcript  as metadata. This whole functionality is built packaged into a Rocket.Chat.App, which can be configured to use the transcription provider of user's choice.

## 📝 Deliverables

The deliverables of the project are as follows:

- [x] To be able to transcribe the audio files on server side & store the transcript metadata on demand.
- [x] Create an efficient API to be able to queue/get transcripts.

- [x] Design & Develop an interactive app interface.
  - Utililsed [Rocket.Chat.Fuselage Monorepo](https://github.com/RocketChat/Rocket.Chat.Fuselage/tree/develop/packages/fuselage-ui-kit) for creating App components.
- [x] Provide the User and option to choose from a variety of API providers for trascription. Currently supported providers are:
  - Assembly AI.
  - Mcirosoft Cognitive Services .
  - & Rev AI.

- [x] Write flexible code so that it's easy to add support for a new provider in the future.

All of the listed deliverables were completed within the GSoC period. YAY !! 🎉

## 📦 Working product

The work can be found here - [App on Github](https://github.com/RocketChat/Apps.SpeechToText). Please refer to the Readme.md for setup.

**I have also written a blog on how it works attached [here](https://reactnativeelements.com/blog/2021/08/12/auto-generation-of-docs).**

## 🚀 Contributions
This is a standalone app built over [Rocket.Chat.Apps-Engine](https://github.com/RocketChat/Rocket.Chat.Apps-engine) & [Rocket.Chat.Apps-Cli](https://github.com/RocketChat/Rocket.Chat.Apps-cli), which can be installed for free from the Rocket.Chat Apps marketplace. It is not a part of the core Rocket.Chat but lives inside the codebase, been provided with the maintainer rights i didn't need to create PR's so here are the commits that sum up the project.

### Pull requests

| Commit Link                                                                                                                                                              | Description                                              | Status    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- | --------- |
| [Setup](https://github.com/RocketChat/Apps.SpeechToText/commit/ffbba97696a6f045496006524b679f58add03900)                                                                                    | [New] Instantiated a boilerplate app using Rocket.Chat CLI             | Approved ✅ |
| [Webhook APi & User settings](https://github.com/RocketChat/Apps.SpeechToText/commit/1d85ba0cca8b5dc3f396ad6881575766e82f8f93)                                                                                    | [New] Added user settings and created Webhook for provider             | Approved ✅ |
| [Message helpers](https://github.com/RocketChat/Apps.SpeechToText/commit/4935f9612772d9854559382f60f50bd633a2610c)                                                                                    | [New] Helper functions for creating and sending status messages  | Approved ✅ |
| [Provider Interface](https://github.com/RocketChat/Apps.SpeechToText/commit/63c312654434090820de1d72d87379562d28396e)                                                                                    | [New] A new interface that can be implemented whenever an API provider is to be added      | Approved ✅ |
| [JWT-implementation](https://github.com/RocketChat/Apps.SpeechToText/commit/c0e8c56ed1678ed6484a1b14a54a7206c30b1d35)                                                                                    | [New] custom implementation of JWT using crypto module for file security        | Approved ✅ |
| [Provider](https://github.com/RocketChat/Apps.SpeechToText/commit/14c918e5f17eb73a5b58a94c95d00f7a8e24d1fa)                                                                                    | [Add] Added AssemblyAI support             | Approved ✅ |
| [Provider](https://github.com/RocketChat/Apps.SpeechToText/commit/36e247285d75df02e4056cb05a052a032c762498)| [Add] Added Microsoft Cognitive Services support | Approved ✅ |
| [Provider](https://github.com/RocketChat/Apps.SpeechToText/commit/67ba4a05df2d5c0bd95e06649a20136d6e6c78db)                                                                                    | [Add] Added support for Rev AI           | Aproved ✅ |
|[Test Mode](https://github.com/RocketChat/Apps.SpeechToText/commit/b731d1257f73dff911102faddb650769391567cc)|[New,Improve] Added a new test mode setting and improved error handling  | Aproved ✅ ||
|[Slash command](https://github.com/RocketChat/Apps.SpeechToText/commit/9ddb9919e2281f678c0a50d34ba8a2118572dc6c)|[Refactor] Refactored slash commands|Aproved ✅ |
|[Bug Fixes](https://github.com/RocketChat/Apps.SpeechToText/commit/2b7ba71f64fb846b824c407f27bdd0615fb94e1d)|[Improve,Refactor] Added error handling layers and comments for readability]|Aproved ✅ ||



Apart from these contributions, I have contributed to other Rocket.Chat projects. They can be summarized as:
| Project                           | Reference                                                                                                                          |
| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Rocket.Chat - main repo | [Pull requests](https://github.com/RocketChat/Rocket.Chat/pulls?q=+is%3Apr+author%3AKartik18g+)                |
| Rocket.Chat.Fuselage         | [Pull requests](https://github.com/RocketChat/Rocket.Chat.Fuselage/pulls?q=+is%3Apr+author%3AKartik18g+) |


## Mentors

I would like to thank my mentors [Marcelo Schmidt](https://github.com/marceloschmidt) & [Douglas Gubert](https://github.com/d-guberta) for helping me reach this milestone and providing me this opportunity. 😄😄

I have not only learned about the Open Source culture and how to write good code but also, learned how the industry works and the import

I would also like to thank [Priya Bihani](https://github.com/PriyaBihani) for her constant support.

## 🔗 Links

<div  align="center">

| **Student**      |                                                    Kartik Gupta                                                     |
| :--------------- | :--------------------------------------------------------------------------------------------------------------------: |
| **Organization** |                           [Rocket.Chat](https://github.com/RocketChat)                           |
| **Project**      | [Speech To Text](https://github.com/RocketChat/Apps.SpeechToText) |
| **GitHub**       |                                       [Kartik18g](https://github.com/Kartik18g)                                        |
| **LinkedIn**     |                                [Kartik Gupta](https://www.linkedin.com/in/kartik-gupta-3275651b8/)                                |
| **Twitter**      |                                     [Gkaartik](https://twitter.com/Gkaartik)                                     |
| **Email**        |                    <a  href="mailto:gupta.kartik18kg@gmail.com">gupta.kartik18kg@gmail.com</a>                     |

</div>

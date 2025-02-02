# Amazon Polly Developer Guide

-----
*****Copyright &copy; Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What Is Amazon Polly?](what-is.md)
+ [How Amazon Polly Works](how-text-to-speech-works.md)
+ [Getting Started with Amazon Polly](getting-started.md)
   + [Step 1: Set Up an AWS Account and Create a User](setting-up.md)
   + [Step 2: Getting Started (Console)](getting-started-console.md)
   + [Step 3: Getting Started (AWS CLI)](getting-started-cli.md)
      + [Step 3.1: Set Up the AWS Command Line Interface (AWS CLI)](setup-aws-cli.md)
      + [Step 3.2: Getting Started Exercise Using the AWS CLI](get-started-cli-exercise.md)
   + [Python Examples](get-started-what-next.md)
+ [Voices in Amazon Polly](voicelist.md)
   + [Bilingual Voices](bilingual-voices.md)
   + [Listening to the Voices](listening-voices.md)
   + [Voice Speed](voice-speed-vip.md)
   + [Languages Supported by Amazon Polly](SupportedLanguage.md)
      + [Phoneme and Viseme Tables for Supported Languages](ref-phoneme-tables-shell.md)
         + [Arabic (arb)](ph-table-arabic.md)
         + [Chinese, Mandarin (cmn-CN)](ph-table-mandarin.md)
         + [Danish (da-DK)](ph-table-danish.md)
         + [Dutch (nl-NL)](ph-table-dutch.md)
         + [English, Australian (en-AU)](ph-table-english-au.md)
         + [English, American (en-US)](ph-table-english-us.md)
         + [English, British (en-GB)](ph-table-english-uk.md)
         + [English, Indian (en-IN)](ph-table-english-in.md)
         + [English, New Zealand (en-NZ)](ph-table-english-nz.md)
         + [English, South African (en-ZA)](ph-table-english-za.md)
         + [English, Welsh (en-GB-WSL)](ph-table-english-wls.md)
         + [French (fr-FR)](ph-table-french.md)
         + [French, Canadian (fr-CA)](ph-table-french-ca.md)
         + [German (de-DE)](ph-table-german.md)
         + [Hindi (hi-IN)](ph-table-hindi.md)
         + [Icelandic (is-IS)](ph-table-icelandic.md)
         + [Italian (it-IT)](ph-table-italian.md)
         + [Japanese (ja-JP)](ph-table-japanese.md)
         + [Korean (ko-KR)](ph-table-korean.md)
         + [Norwegian (nb-NO)](ph-table-norwegian.md)
         + [Polish (pl-PL)](ph-table-polish.md)
         + [Portuguese (pt-PT)](ph-table-portuguese.md)
         + [Portuguese, Brazilian (pt-BR)](ph-table-portuguese-br.md)
         + [Romanian (ro-RO)](ph-table-romanian.md)
         + [Russian (ru-RU)](ph-table-russian.md)
         + [Spanish (es-ES)](ph-table-spanish.md)
         + [Spanish, Mexican (es-MX)](ph-table-mexican.md)
         + [Spanish, US (es-US)](ph-table-spanish-us.md)
         + [Swedish (sv-SE)](ph-table-swedish.md)
         + [Turkish (tr-TR)](ph-table-turkish.md)
         + [Welsh (cy-GB)](ph-table-welsh.md)
+ [Neural TTS](NTTS-main.md)
   + [Neural Voices](ntts-voices-main.md)
   + [NTTS Newscaster Speaking Style](ntts-speakingstyles.md)
+ [Speech Marks](speechmarks.md)
   + [Speech Mark Types](using-speechmarks1.md)
      + [Visemes and Amazon Polly](viseme.md)
   + [Using Speech Marks](using-speechmarks.md)
      + [Speech Mark Examples](speechmarkexamples.md)
   + [Requesting Speech Marks (Console)](speechmarksconsole.md)
+ [Generating Speech from SSML Documents](ssml.md)
   + [Reserved Characters in SSML](escapees.md)
   + [Using SSML (Console)](ssml-to-speech-console.md)
   + [Using SSML (AWS CLI)](ssml-synthesize-speech-cli.md)
   + [Supported SSML Tags](supportedtags.md)
+ [Managing Lexicons](managing-lexicons.md)
   + [Applying Multiple Lexicons](lexicons-applying.md)
   + [Managing Lexicons Using the Amazon Polly Console](managing-lexicons-console.md)
   + [Managing Lexicons Using the AWS CLI](managing-lexicons-cli.md)
      + [Using the PutLexicon Operation](gs-put-lexicon.md)
      + [Using the GetLexicon Operation](gs-get-lexicon.md)
      + [Using the ListLexicons Operations](gs-list-lexicons.md)
      + [Using the DeleteLexicon Operation](gs-delete-lexicon.md)
+ [Creating Long Audio Files](asynchronous.md)
   + [Setting Up the IAM Policy for Asynchronous Synthesis](asynchronous-iam.md)
   + [Creating Long Audio Files (Console)](longer-console.md)
   + [Creating Long Audio Files (CLI)](longer-cli.md)
+ [Code and Application Examples](samples-and-examples.md)
   + [Sample Code](sample-code-overall.md)
      + [Java Samples](java-samples-overall.md)
         + [DeleteLexicon](DeleteLexiconSample.md)
         + [DescribeVoices](DescribeVoicesSample.md)
         + [GetLexicon](GetLexiconSample.md)
         + [ListLexicons](ListLexiconsSample.md)
         + [PutLexicon](PutLexiconSample.md)
         + [StartSpeechSynthesisTask](StartSpeechSynthesisTask.md)
         + [Speech Marks](SynthesizeSpeechMarksSample.md)
         + [SynthesizeSpeech](SynthesizeSpeechSample.md)
      + [Python Samples](python-samples-overall.md)
         + [DeleteLexicon](DeleteLexiconPython.md)
         + [GetLexicon](GetLexiconSamplePython.md)
         + [ListLexicon](ListLexiconSamplePython.md)
         + [PutLexicon](PutLexiconSamplePython.md)
         + [StartSpeechSynthesisTask](StartSpeechSynthesisTaskSamplePython.md)
         + [SynthesizeSpeech](SynthesizeSpeechSamplePython.md)
   + [Example Applications](examples-for-using-polly.md)
      + [Python Example (HTML5 Client and Python Server)](examples-python.md)
         + [Python Example: HTML5 User Interface (index.html)](example-html-app.md)
         + [Python Example: Python Server Code (server.py)](example-Python-server-code.md)
      + [Java Example](examples-java.md)
      + [iOS Example](examples-ios.md)
      + [Android Example](examples-android.md)
+ [Amazon Polly for Windows SAPI Compliant Applications](sapi-plugin.md)
   + [Installing and Configuring Amazon Polly for Windows (SAPI)](install-voice-plugin2.md)
   + [Using Amazon Polly in Applications](pollywindowsplugin.md)
+ [The AWS for WordPress Plugin](plugin.md)
   + [Installation Prerequisites](WordPressPlugin-prerequisites.md)
   + [Installing and Configuring the Plugin](WordPressPlugin-install.md)
   + [Customizing Your WordPress Page](CustomizingWordPress.md)
   + [Podcasting with Amazon Pollycast](pollycast-podcast.md)
   + [Storing Audio Files](pollycast.md)
+ [Quotas in Amazon Polly](limits.md)
+ [Security in Amazon Polly](security.md)
   + [Data Protection in Amazon Polly](data-protection.md)
      + [Encryption at Rest](encryption-at-rest.md)
      + [Encryption in Transit](encryption-in-transit.md)
      + [Internetwork Traffic Privacy](internetwork-traffic-privacy.md)
   + [Identity and Access Management in Amazon Polly](security-iam.md)
      + [How Amazon Polly Works with IAM](security_iam_service-with-iam.md)
      + [Amazon Polly Identity-Based Policy Examples](security_iam_id-based-policy-examples.md)
      + [Amazon Polly API Permissions: Actions, Permissions, and Resources Reference](api-permissions-reference.md)
   + [Logging and Monitoring in Amazon Polly](sec-logging.md)
   + [Compliance Validation for Amazon Polly](AMAZON-POLLY-compliance.md)
   + [Resilience in Amazon Polly](disaster-recovery-resiliency.md)
   + [Infrastructure Security in Amazon Polly](infrastructure-security.md)
   + [Security Best Practices for Amazon Polly](security-best-practices.md)
+ [Logging Amazon Polly API Calls with AWS CloudTrail](logging-using-cloudtrail.md)
+ [Integrating CloudWatch with Amazon Polly](cloud-watch.md)
+ [Amazon Polly API Reference](API_Reference.md)
   + [Actions](API_Operations.md)
      + [DeleteLexicon](API_DeleteLexicon.md)
      + [DescribeVoices](API_DescribeVoices.md)
      + [GetLexicon](API_GetLexicon.md)
      + [GetSpeechSynthesisTask](API_GetSpeechSynthesisTask.md)
      + [ListLexicons](API_ListLexicons.md)
      + [ListSpeechSynthesisTasks](API_ListSpeechSynthesisTasks.md)
      + [PutLexicon](API_PutLexicon.md)
      + [StartSpeechSynthesisTask](API_StartSpeechSynthesisTask.md)
      + [SynthesizeSpeech](API_SynthesizeSpeech.md)
   + [Data Types](API_Types.md)
      + [Lexicon](API_Lexicon.md)
      + [LexiconAttributes](API_LexiconAttributes.md)
      + [LexiconDescription](API_LexiconDescription.md)
      + [SynthesisTask](API_SynthesisTask.md)
      + [Voice](API_Voice.md)
+ [Document History for Amazon Polly](doc-history.md)
+ [AWS glossary](glossary.md)
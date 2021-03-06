## Human Interface Guidelines

### iOS设计主题：

* Clarity
* Deference
* Depth

### 设计原则：

* Aesthetic Integrity-审美诚信
* Consistency-一致性
* Direct Manipulation-直接操纵
* Feedback-反馈
* Metaphors-隐喻
* User Control

### UIKit

* 大多数iOS应用程序都是使用UIKit的组件构建的，UIKit是一个定义通用界面元素的编程框架。该框架使应用程序在整个系统中实现一致的外观，同时提供高水平的自定义。

### Loading

当内容加载时，空白或静态屏幕可能会使您的应用程序被冻结，从而导致混淆和沮丧，并可能导致人们离开您的应用。

* Make it clear when loading is occurring.
  * At minimum, show an activity spinner that communicates something is happening. Even better, display explicit progress so users can gauge how long they’ll be waiting.
* Show content as soon as possible. 
  * 在看到他们期望的屏幕之前，不要让人们等待内容加载。立即显示屏幕，并使用占位符文本，图形或动画来确定内容尚不可用的位置。在内容加载时替换这些占位符元素。尽可能在后台预加载即将播放的内容，例如在播放动画或用户正在导航关卡或菜单时。
* Educate or entertain people to mask loading time.
* Customize loading screens. 

### Modality

* 帮助人们专注于一个独立的任务或一组密切相关的选项
* 确保人们接收并在必要时对关键信息采取行动
* 使用Modality时，要有意义。
  * 只有当人们的注意力集中在做出选择或执行与当前任务不同的任务时，才能创建模态体验。模式经验使人们脱离当前的背景并需要采取行动解雇，因此只有在提供明确的利益时才使用它。
* 保留提供必要和理想的可操作信息的警报
  * 通常，会出现警报，因为出现了问题。由于警报会中断体验并需要点击才能解除，因此人们必须认为入侵是有道理的。有关指导，请参阅警报。
* 保持模态任务的简单，简短和狭隘。
  * 如果模态任务过于复杂，人们可能会在进入模态文时忽略他们暂停的任务。
  * 如果模态任务必须包含子视图，请提供层次结构中的单个路径以及完成的明确路径。除完成任务外，请避免使用“完成”按钮。
* 始终包含一个取消模态视图的按钮。
* 必要时，通过在关闭模态视图之前获得确认来帮助人们避免数据丢失。
* 不要显示弹出窗口顶部显示的卡片
* 通常，显示标识模态任务的标题。
  * 当人们进入模态任务时，他们会从之前的上下文中切换出来，因此最好使新的上下文清晰。您还可以在视图的其他部分中提供更全面描述任务或提供指导的文本。
* 使用您的应用协调模态视图外观。
* 选择在您的应用中有意义的模态转换样式。

### Navigation

人们往往不知道应用程序的导航，直到它不符合他们的期望。您的工作是以支持应用程序结构和目的的方式实现导航，而不会引起注意。导航应该感觉自然和熟悉，不应该主导界面或从内容中吸引焦点。

* 始终提供明确的路径
  * 人们应该始终知道他们在您的应用中的位置以及如何到达下一个目的地。无论导航风格如何，通过内容的路径都必须符合逻辑，可预测且易于遵循。
* Design an information structure that makes it fast and easy to get to content.
* 使用触摸手势创建流动性。
  * 最小的摩擦力轻松移动界面。例如，您可以让人们从屏幕侧面滑动以返回上一个屏幕。
* 使用标准导航组件。
  * 尽可能使用标准导航控件，例如页面控件，选项卡栏，分段控件，表视图，集合视图和拆分视图。用户已经熟悉这些控件，并且会直观地了解如何绕过您的应用。
* 使用导航栏遍历数据层次结构
  * 导航栏的标题可以显示层次结构中的当前位置，后退按钮可以轻松返回到先前的位置。
* Use a tab bar to present peer categories of content or functionality. 
  * A tab bar可让人们快速轻松地在不同类别之间切换，无论当前位置如何。
* Use a page control when you have multiple pages of the same type of content.

### Onboarding

* Provide a launch screen. 
* 以适当的横竖屏方式展示。
* Get to the action quickly. 
  * 如果有教程，那么可以跳过
* 预计需要帮助。
  * 积极寻找人们可能被卡住的时间。例如，游戏可以在暂停或角色没有前进时随便显示有用的提示。让用户重播教程，以防他们第一次错过任何内容。
* 坚持教程中的要点
  * 为初学者提供指导是好的，但教育并不能代替优秀的应用程序设计。
* Make learning fun and discoverable-让学习变得有趣和可被发现
  * 使用动画和交互性逐步和上下文教学。避免显示看似互动的屏幕截图。
* 避免事先询问设置信息
  * 人们希望应用能够正常运作。为大多数人设计您的应用程序，让少数想要不同配置的应用程序调整设置以满足他们的需求。尽可能从设备设置和默认值或通过同步服务（如iCloud）派生设置信息。
* 当您的应用重新启动时，恢复以前的状态。
  * 不要让人们回溯到您应用中的先前位置。保留并恢复您应用的状态，以便他们可以从中断的地方继续。
* 不要让人们过快或过于频繁地为您的应用评分
  * 过快或过于频繁地要求评级是令人讨厌的，并且会减少您收到的有用反馈的数量。为了鼓励考虑周全的反馈，在要求评级之前，让人们有时间对您的应用发表意见。始终提供退出评级提示的方法，并且永远不要强迫用户为您的应用评分。
* 不要鼓励重启。
  * 重新启动需要时间，使您的应用程序看起来不可靠且难以使用。

### Requesting Permission

* Request personal data only when your app clearly needs it.
  * 对个人信息的请求持怀疑态度是很自然的，特别是在没有明显需要的情况下。确保仅在人们使用明确需要个人数据的功能时才会发出权限请求。例如，应用可能仅在激活位置跟踪功能时请求访问当前位置。
* Explain why your app needs the information.
* 仅在您的应用运行所需时才会在启动时请求权限。
* 不要不必要地请求位置信息。
* Use the system-provided alert.

### Settings

* 推断你可以从系统中得到什么。
  * 如果您需要有关用户，设备或环境的信息，请尽可能向系统查询，而不是询问用户。
* 仔细确定应用程序中配置选项的优先级。
  * 您的应用程序的主屏幕是一个选择必要或经常更改的好地方。辅助屏幕更适合仅偶尔更改的选项。
* 在“设置”中公开不经常更改的配置选项。
* 在适当的时候提供设置的快捷方式。

### Authentication

* 如果您不使用Apple登录，请使用密码自动填充。
* 尽可能延迟登录。
* 说明身份验证的好处以及如何注册您的服务。
* 通过显示适当的键盘来最小化数据输入。
* 尽可能支持生物识别身份验证。

### Data Entry

无论是点击界面元素还是使用键盘，输入信息都是一个繁琐的过程。当一个应用程序通过在做任何有用的事情之前要求大量输入来减慢这个过程时，人们可能会很快气馁，甚至可能完全放弃应用程序。

* 如果可能，提出选择。
  * 考虑使用选择器或表而不是文本字段，因为从预定义选项列表中选择比键入响应更容易。
* 尽可能从系统获取信息。
* 提供合理的默认值。
* 仅在收集所需值后启用提升。
* 动态验证字段值。
  * 填写冗长的表格后，如果必须返回并纠正错误，那将是令人沮丧的。只要有可能，请在输入后立即检查字段值，以便用户立即纠正它们。
* 仅在必要时才需要字段值。
* 通过值列表轻松导航。
* 在文本字段中显示提示以帮助沟通目的。

### Feedback

反馈可以帮助人们了解应用正在做什么，发现他们下一步可以做什么，并了解行动的结果。

* 不显眼地将状态和其他类型的反馈集成到您的界面中。
  * 理想情况下，用户无需采取行动或中断即可获取重要信息。例如，邮件在浏览邮件邮箱时巧妙地在工具栏中显示状态信息。此信息不会与屏幕上的主要内容竞争，但可以随时快速查看。
* 避免不必要的警报
  * 警报是一种强大的反馈机制，但应仅用于提供重要且理想的可操作信息。如果人们看到太多不包含重要信息的警报，他们很快就会学会忽略未来的警报。

### Gestures

人们通过在触摸屏上执行手势来与iOS设备进行交互。这些手势引发了与内容的紧密个人联系，增强了对屏幕对象的直接操纵感。

* 作为一般规则，使用标准手势。
* 避免使用标准手势执行非标准操作。
* 避免干扰系统范围的屏幕边缘手势。
* 提供快捷手势以补充而非替换基于界面的导航和操作。
  * 只要有可能，提供一种简单，可见的方式来导航或执行操作，即使这意味着额外的一两个点击。

### Undo and Redo

许多应用程序允许人们摇动设备以撤消和重做某些操作，例如键入或删除。以这种方式启动时，警报会要求用户确认或取消撤消或重做操作。

* 简要而准确地描述要撤消或重做的操作。
* 如果您使用摇动手势进行撤消和重做，请不要将其用于其他操作。
* 谨慎提供撤消和重做按钮。
* 仅在当前上下文中执行撤消和重做操作：
  * 撤消和重做应该对当前上下文有明确而直接的影响，而不是早期的上下文。

### Notifications

无论设备是锁定还是正在使用，应用都可以随时使用通知提供及时和重要的信息。

* 提供有用的信息性通知。
  * 人们可以通知通知以获得快速更新，因此专注于提供有价值的信息。使用完整的句子，句子大小写，正确的标点符号，并且不要截断您的消息 - 系统会在必要时自动执行此操作。
* 即使用户没有响应，也不要为同一件事发送多个通知。
  * People attend to notifications at their convenience. If you send multiple notifications for the same thing, you fill up Notification Center, and users may turn off notifications from your app.
* 请勿包含您的应用名称或图标。
  * 系统会在每个通知的顶部自动显示此信息。
* 提供描述性文本，以便在隐藏通知预览时显示。
* 提供声音以补充您的通知。
* 考虑提供详细视图。
* 提供直观，有益的行动。
* 避免提供破坏性行为。

### Badging

* 使用标记来补充通知，而不是表示关键信息。
* 使用标记仅用于通知目的。
* 保持徽章最新。

### Ratings and Reviews

* 仅在用户证明与您的应用互动后才要求评分。
* 不要打断用户，特别是当他们执行时间敏感或压力很大的任务时。
* Don’t be a pest.
* 首选系统提供的提示。
  * 系统的评级提示提供熟悉，高效的体验，旨在以最小的影响吸引用户。
* 请勿使用按钮或其他控件来请求反馈。
  * 由于系统限制了评级提示发生的频率，因此尝试响应控件请求反馈可能导致不显示评级提示。

### 一般布局注意事项

* Ensure that primary content is clear at its default size.
* 在整个应用中保持整体一致的外观。
* 使用视觉重量和平衡来传达重要性。大件物品吸引眼球，看起来比较小物品更重要。
* 使用对齐可以简化扫描并与组织和层次结构进行通信。
* 如果可能，支持纵向和横向。
* 准备好进行文本大小的更改。
* 为交互式元素提供充足的触摸目标。44pt x 44pt的最小可点击区域.
* 在多个设备上预览您的应用。
* 在较大的设备上显示文本时应用可读性边距。

### 适应语境的变化

* 在上下文变化期间保持对当前内容的关注。

  * 内容是您的最高优先级。在环境变化时改变焦点可能令人迷茫和令人沮丧，并且可能让人觉得他们失去了对应用程序的控制。

* 避免无偿的布局更改。

* 如果您的应用以单一方向运行至关重要，请同时支持这两种变体。

* 根据上下文自定义应用程序对轮换的响应。

* 确保您的应用在iPad上运行，而不仅仅在iPhone上运行。

### 设计全屏体验



![image-20190630174404232](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630174404232.png)

* 插入全宽按钮。
  * 延伸到屏幕边缘的按钮可能看起来不像按钮。尊重全宽按钮两侧的标准UIKit边距。
* 请勿掩盖或特别注意按键显示功能。
* 请注意状态栏的高度。
* 如果您的应用当前隐藏了状态栏，请重新考虑全屏iPhone的决定。
* 允许自动隐藏指示符以便谨慎访问主屏幕。

### Animation

整个iOS中美丽，微妙的动画构建了人与屏幕内容之间的视觉连接感。如果使用得当，动画可以传达状态，提供反馈，增强直接操控感，并帮助用户可视化他们的行为结果。

* 明智地使用动画和动作效果。
  * 不要为了使用动画而使用动画。过度或无偿的动画可能会让人感到脱节或分心，特别是在没有提供身临其境体验的应用中。
* 力求现实主义和信誉。
  * 人们倾向于接受艺术许可，但是当运动没有意义或似乎违背物理定律时，他们会感到迷失方向。
* 使用一致的动画。
  * 熟悉，流畅的体验让用户保持参与。
* 使动画可选。

### Terminology（术语）

您应用中的每个字都是与用户对话的一部分。使用此对话可以帮助他们在您的应用中感到舒适。

* 使用熟悉，易懂的单词和短语
* Keep interface text clear and concise. 
* 适当地识别互动元素。
  * 人们应该能够一眼就看出元素的作用。标记按钮和其他交互元素时，请使用动作谓词，例如“连接”，“发送”和“添加”。
* 避免使用可能听起来光顾的语言。
* 力求非正式，友好的语气。
* 使用幽默时要小心。
* 使用相关且一致的语言和图像。
* 准确地参考日期。

### Typography（排版）

旧金山（SF）是iOS中的系统字体。此字体的字体经过优化，可为您的文本提供无与伦比的易读性，清晰度和一致性。

* 强调重要信息。
* 如果可能，请使用单一字体。
* 尽可能使用内置文本样式。
  * 内置的文本样式允许您以视觉上不同的方式表达内容，同时保持最佳的易读性。
* 确保自定义字体清晰易读。
* 在接口模型中使用正确的字体变体

### App Icon

每个应用程序都需要一个美丽而令人难忘的图标，吸引App Store的注意力，并在主屏幕上脱颖而出。您的图标是第一次与您的应用程序进行通信的机会。它也会出现在整个系统中，例如“设置”和搜索结果中。

* 拥抱简约。
  * 找到一个能够捕捉应用程序本质的元素，并以简单，独特的形状表达该元素。谨慎添加细节。如果图标的内容或形状过于复杂，则难以辨别细节，尤其是在较小尺寸时。
* 提供单一焦点
  * 设计一个带有单个中心点的图标，可以立即捕获注意力并清楚地识别您的应用。
* 设计一个可识别的图标。
  * 人们不应该分析图标来弄清楚它代表什么。
* 保持背景简单，避免透明度。
  * 确保您的图标不透明，并且不会使背景混乱。
* 只有在文字必不可少或是徽标的一部分时才使用。
  * 应用程序的名称显示在主屏幕上的图标下方。不要包含重复名称的非必要词语或告诉人们如何处理您的应用，例如“观看”或“播放”。如果您的设计包含任何文字，请强调与您的应用提供的实际内容相关的字词。
* 不要包含照片，屏幕截图或界面元素。
  * 小尺寸的照片细节很难看到。屏幕截图对于应用程序图标来说过于复杂，通常无法帮助您传达应用程序的用途。
* 针对不同的壁纸测试您的图标。

### Launch Screen

当您的应用启动时，系统会立即显示启动屏幕，并立即将其替换为应用的第一个屏幕，从而给您的应用提供快速响应的印象。发布屏幕不是艺术表达的机会。它仅用于增强您的应用程序的感知，以便快速启动并立即使用。每个应用程序都必须提供启动屏幕。

* 设计一个与应用程序的第一个屏幕几乎相同的启动屏幕。
* 避免在启动屏幕上包含文字。
* 淡化发布。
* 不要做广告。

### Navigation Bars

* 在显示全屏内容时，请考虑暂时隐藏导航栏。

### Navigation Bar Titles

* 考虑在导航栏中显示当前视图的标题。
  * 在大多数情况下，标题可以帮助人们理解他们正在看的内容。
* 当您想要特别强调上下文时，请使用大标题。
* 考虑隐藏大标题导航栏的边框。

### Navigation Bar Controls-导航栏控件

* 避免拥挤太多控件的导航栏。
  * 通常，导航栏应该只包含视图的当前标题，后退按钮和一个管理视图内容的控件。如果在导航栏中使用分段控件，则栏不应包含标题或除分段控件之外的任何控件。
* 使用标准后退按钮。
  * 人们知道标准后退按钮可以让他们回溯信息层次结构。但是，如果您实现自定义后退按钮，请确保它仍然看起来像后退按钮，行为直观，与您的界面的其余部分匹配，并在整个应用程序中始终如一地实施。
* 不要包含多段面包屑路径。
  * 后退按钮始终执行单个操作 - 返回上一个屏幕。
* 给文本标题的按钮足够的空间。 
* 考虑在导航栏中使用分段控件来展平应用程序的信息层次结构。

### Search Bars

搜索栏允许人们通过在字段中键入文本来搜索大量值。搜索栏可以单独显示，也可以在导航栏或内容视图中显示。当在导航栏中显示时，搜索栏可以固定到导航栏，以便始终可以访问，或者可以折叠直到用户向下滑动以显示它。

* 使用搜索栏而不是文本字段来实现搜索。
* 启用“清除”按钮。
* 适当时启用“取消”按钮。
* 如有必要，请在搜索栏中提供提示和上下文。
* 考虑在搜索栏下方提供有用的快捷方式和其他内容。使用

### Scope Bars-范围栏

可以将范围栏添加到搜索栏以让人们优化搜索范围。

* 有利于改进搜索结果，包括范围栏。

### Status Bars

状态栏显示在屏幕的上边缘，并显示有关设备当前状态的有用信息，如时间，移动电话运营商，网络状态和电池电量。状态栏中显示的实际信息因设备和系统配置而异。

* 使用系统提供的状态栏。
  * 人们希望状态栏在整个系统范围内保持一致。请勿使用自定义状态栏替换它。
* 使用您的应用程序设计协调状态栏样式。
* 状态栏下隐藏的内容。
  * 默认情况下，状态栏的背景是透明的，允许下方的内容显示。保持状态栏可读，并不暗示其背后的内容是交互式的。
* 在显示全屏媒体时，请考虑暂时隐藏状态栏。
  * 当用户尝试关注媒体时，状态栏可能会分散注意力。暂时隐藏这些元素以提供更加身临其境的体验。
* 避免永久隐藏状态栏。
* 使用状态栏表示网络活动。

### Tab Bars

标签栏显示在应用程序屏幕的底部，可以在应用程序的不同部分之间快速切换。标签栏是半透明的，可以具有背景色调，在所有屏幕方向上保持相同的高度，并且在显示键盘时隐藏。标签栏可能包含任意数量的标签，但可见标签的数量因设备大小和方向而异。如果由于水平空间有限而无法显示某些选项卡，则最终的可见选项卡将变为“更多”选项卡，从而在单独的屏幕上显示列表中的其他选项卡。

* 通常，使用标签栏在应用级别组织信息。
* 严格使用标签栏进行导航。
  * 标签栏按钮不应用于执行操作。如果需要提供作用于当前视图中元素的控件，请改用工具栏。
* 避免使用太多标签。
  * 每个附加选项卡都会减少用于选择选项卡的可点击区域，并增加应用程序的复杂性，从而使查找信息变得更加困难。虽然“更多”选项卡可以显示额外的选项卡，但这需要额外的点击，并且空间使用率很低。
  * 选项卡太少也可能是一个问题，因为它可能会使您的界面显示为断开连接。通常，在iPhone上使用三到五个标签。
* 当人们导航到您应用中的不同区域时，请勿隐藏标签栏。
  * 标签栏为您的应用启用全局导航，因此它应该始终可见。例外情况是模态视图。因为模态视图为人们提供了一个单独的体验，当他们完成时他们会忽略，这不是应用程序整体导航的一部分。
* 当功能不可用时，请勿删除或禁用选项卡。
  * 如果选项卡在某些情况下可用但在其他情况下不可用，则应用程序的界面将变得不稳定且不可预测。确保始终启用所有选项卡，并解释选项卡内容不可用的原因。例如，如果iOS设备上没有歌曲，则音乐应用中的“我的音乐”选项卡会说明如何下载歌曲。
* 始终在附加视图中切换上下文。
  * 要保持界面可预测，选择选项卡应始终影响直接连接到选项卡栏的视图，而不是影响屏幕上其他位置的其他视图。
* 确保标签栏图标在视觉上一致且平衡。
* 使用徽章进行不引人注目的沟通。

### Toolbars

工具栏显示在应用程序屏幕的底部，其中包含用于执行与当前视图或其中内容相关的操作的按钮。工具栏是半透明的，可能具有背景色调，并且在人们不太可能需要它们时经常隐藏。

* 提供相关工具栏按钮。
* 考虑图标或文本标题按钮是否适合您的应用。
* 避免在工具栏中使用分段控件。
  * 分段控件允许人们切换上下文，而工具栏特定于当前屏幕。如果您需要提供切换上下文的方法，请考虑使用标签栏。
* 给文本标题的按钮足够的空间。

### Action Sheets

操作表是响应控件或操作而显示的特定警报样式，并呈现与当前上下文相关的一组两个或更多选项。使用操作表让人们在执行潜在的破坏性操作之前启动任务或请求确认。

在较小的屏幕上，操作表从屏幕底部向上滑动。在较大的屏幕上，一个操作表一下子显示为一个弹出窗口。

* 如果增加清晰度，请提供“取消”按钮。
* 使破坏性选择突出（prominent）。
* 避免在操作表中启用滚动。

### Activity Views

活动是在当前上下文中有用的任务，例如“复制”，“收藏夹”或“查找”。一旦启动，活动可以立即执行任务，或在继续之前询问更多信息。活动由活动视图管理，活动视图显示为工作表或弹出窗口，具体取决于设备和方向。使用活动可以让人们访问您的应用可以执行的自定义服务或任务。

* 设计简单的模板图像来表示您的自定义活动。
* 简明扼要地描述您的任务的工艺活动标题。
* 确保活动适合当前上下文。
* 使用“操作”按钮显示活动视图。

### Alerts

警报传达与应用程序或设备状态相关的重要信息，并经常请求反馈。警报由标题，可选消息，一个或多个按钮以及用于收集输入的可选文本字段组成。除了这些可配置元素之外，警报的视觉外观是静态的，无法自定义。

* Minimize alerts. 
  * 警报会破坏用户体验，只应在重要情况下使用，例如确认购买和破坏性操作（例如删除）或通知人们有关问题。警报的频率很低，有助于确保人们认真对待。确保每个警报提供关键信息和有用的选择。
* Test the appearance of alerts in both orientations.
  * 在横向模式和纵向模式下，警报可能会有所不同。优化警报文本，使其在任何方向上都能很好地读取而无需滚动。
* 编写简短的描述性多字警报标题。
* 如果你必须提供信息，请写短，完整的句子。
* 避免听到指责，判断或侮辱。
* 避免解释警报按钮。
* 通常，使用双按钮警报。
  * 双键警报提供两种选择之间的简单选择。单键警报通知，但无法控制情况。具有三个或更多按钮的警报会产生复杂性并且可能需要滚动，这是一种糟糕的用户体验。如果您发现需要两个以上的选择，请考虑使用操作表。
* 提供警报按钮简洁，合乎逻辑的标题。
  * 最佳按钮标题由一个或两个单词组成，用于描述选择按钮的结果。与所有按钮标题一样，使用标题样式大小写并且没有结束标点符号。
* 将按钮放在人们期望的位置。
  * 一般来说，人们最有可能点击的按钮应该在右边。取消按钮应始终位于左侧。
* 标签取消按钮适当。
  * A button that cancels an alert’s action should always be labeled Cancel.
* 识别破坏性按钮。
  * 如果警报按钮导致破坏性操作（例如删除内容），请将按钮的样式设置为“破坏性”，以便系统进行适当的格式化。
* 允许用户通过退出主屏幕取消提醒。
  * 在显示警报时访问主屏幕将退出应用程序。它还应该产生与点击取消按钮相同的效果 - 也就是说，警报被解除而不执行任何操作。如果您的警报没有“取消”按钮，请考虑在代码中实施取消操作，该操作在某人退出您的应用时运行。

### Collections

Collections管理一组有序的内容，例如一组照片，并以可自定义和高度可视化的布局呈现。由于Collections不强制执行严格的线性格式，因此它特别适合显示大小不同的项目。一般来说，收藏品非常适合炫耀基于图像的内容。可选地，可以实现背景和其他装饰视图以在视觉上区分项目的子集。

* 当标准行或网格布局足够时，避免创建激进的新设计。
  * 集合应该增强用户体验，而不是成为关注的焦点。可以轻松选择项目。如果在您的收藏中点击某个项目很困难，那么在达到他们想要的内容之前，人们会感到沮丧并失去兴趣。在内容周围使用足够的填充以保持布局清洁并防止内容重叠。
* 考虑使用表而不是文本集合
  * 当文本信息显示在可滚动列表中时，查看和摘要文本信息通常更简单，更有效。
* 进行动态布局更改时要小心。
  * 可以随时更改集合的布局。如果您在人们查看和与之交互时动态更改布局，请确保更改有意义且易于跟踪。无动机的布局更改可能会使您的应用程序看起来难以预测且难以使用。

### Popovers（弹出窗口）

弹出框是一种瞬态视图，当您点击控件或区域时，它会显示在屏幕上的其他内容上方。通常，弹出框包括指向其出现位置的箭头。弹壳可以是非模态的或模态的。通过点击屏幕的另一部分或弹出窗口上的按钮来解除非模态弹出窗口。通过点击弹出窗口上的取消或其他按钮可以解除模态弹出窗口。

弹出窗口最适合大屏幕，可以包含各种元素，包括导航栏，工具栏，标签栏，表格，集合，图像，地图和自定义视图。当弹出窗口可见时，通常会禁用与其他视图的交互，直到弹出窗口被取消。

* 避免在iPhone上显示弹出窗口。

### Scroll Views

滚动视图允许用户浏览大于可见区域的内容，例如文档中的文本或图像集合。当人们轻扫，轻弹，拖动，点击和捏合时，滚动视图会跟随手势，以自然的方式显示或缩放内容。

* 适当支持缩放行为。
* 当滚动视图处于分页模式时，请考虑显示页面控制元素。
* 不要将滚动视图放在另一个滚动视图中。
* 通常，一次显示一个滚动视图。

### Split Views

拆分视图管理两个并排的内容窗格的显示，主窗格中包含持久内容，辅助窗格中包含相关信息。每个窗格都可以包含各种元素，包括导航栏，工具栏，标签栏，表格，集合，图像，地图和自定义视图。

* 选择适合您内容的拆分视图布局。
* 持续突出显示主窗格中的活动选择。
* 通常，将导航限制在拆分视图的一侧。
* 提供多种方法来访问隐藏的主窗格。

### Tables

表格将数据显示为可以分为部分或组的滚动单列行列表。使用表格以列表的形式干净，高效地显示大量或少量信息。一般而言，表格是基于文本的内容的理想选择，并且通常在分割视图的一侧显示为导航手段，相反的内容显示在另一侧。

* Think about table width.
  * 薄表可能导致截断和包装，使得它们难以在远处快速读取和扫描。宽表也可能难以阅读和扫描，并且可能从内容中占用空间。
* Begin showing table content quickly. 
  * 在显示内容之前，不要等待大量的表内容加载。立即使用文本数据填充屏幕行，并显示更复杂的数据（如图像）。这种技术可以立即为人们提供有用的信息，并提高应用程序的感知响应能力。
* 在内容加载时传达进度。
  * 如果表格的数据需要一段时间才能加载，请显示进度条或旋转活动指示符，以向用户保证您的应用仍在运行。
* 保持内容新鲜。
  * 请考虑定期更新表格内容以反映较新的数据。只是不要改变滚动位置。相反，将内容添加到表的开头或结尾，让人们在准备好时滚动到它。某些应用会在添加新数据时显示指示符，并提供向右跳转的控件
* 避免将索引与包含右对齐元素的表行组合。

![image-20190630223459685](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630223459685.png)

* 保持文字简洁，以避免剪裁。
* 考虑使用“删除”按钮的自定义标题。
  * 果某行支持删除并且有助于提供清晰度，请将系统提供的删除标题替换为自定义标题。
* 在做出选择时提供反馈。
  * 人们期望在其内容被点击时短暂突出显示一行。然后，人们期望出现新的视图或者要改变的东西，例如出现的复选标记，表示已经进行了选择。
* 为非标准表行设计自定义表格单元格样式。
  * 标准样式非常适合在各种常见场景中使用，但某些内容或整体应用程序设计可能需要大量自定义的表格外观。

### Text Views

文本视图显示多行样式的文本内容。文本视图可以是任何高度，并在内容扩展到视图之外时启用滚动。默认情况下，文本视图中的内容是左对齐的，并使用黑色的系统字体。如果文本视图可编辑，则在视图内部点击时会出现键盘。

* 保持文字清晰。
* 显示适当的键盘类型。

### Web Views

Web视图直接在您的应用中加载和显示丰富的Web内容，例如嵌入式HTML和网站。例如，Mail使用Web视图在消息中显示HTML内容。

* 适当时启用前进和后退导航。
  * Web视图支持前向和后向导航，但默认情况下禁用此行为。如果用户将使用您的Web视图访问多个页面，请启用前进和后退导航，并提供相应的控件以启动这些功能。
* 避免使用Web视图来构建Web浏览器。
  * 使用Web视图让人们在不离开应用程序上下文的情况下短暂访问网站很好，但Safari是人们在iOS上浏览网页的主要方式。尝试在您的应用程序中复制Safari的功能是不必要的，并且不鼓励。

### Buttons

按钮启动特定于应用程序的操作，具有可自定义的背景，并且可以包含标题或图标。

* 在标题中使用动词。
* 使用title-case作为标题。
  * 将除了文章，协调连词和四个或更少字母的介词之外的每个单词大写。
* 保持标题简短。
* 请考虑仅在必要时添加边框或背景。
  * 默认情况下，系统按钮没有边框或背景。然而，在一些内容区域中，边界或背景是表示交互性所必需的。在手机应用程序中，带边框的数字键加强了传统的拨打电话模式，而“呼叫”按钮的背景提供了一个易于击中的引人注目的目标。

### Detail Disclosure Buttons-细节披露按钮

“详细信息披露”按钮可打开视图（通常是模态视图），其中包含与屏幕上特定项目相关的其他信息或功能。虽然您可以在任何类型的视图中使用它们，但详细信息披露按钮通常用于表中以访问有关特定行的信息。

* 在表格中适当使用详细信息披露按钮。

### Info Buttons

* 在翻转视图后，“信息”按钮会显示有关应用程序的配置详细信息，有时位于当前视图的背面。

### Add Contact Buttons

* 除“添加联系人”按钮外，还允许键盘输入。
  * “添加联系人”按钮提供了键入联系人信息的替代方法，而非替代方法。

### Context Menus-内容菜单

![image-20190630224545159](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630224545159.png)

上下文菜单类似于Peek和Pop，但有两个主要区别：

* 所有运行iOS 13及更高版本的设备都可以使用上下文菜单; Peek和Pop仅适用于支持3D Touch的设备。
* 上下文菜单立即显示上下文相关的命令; Peek和Pop需要向上滑动才能查看命令。

### Edit Menus-编辑菜单

![image-20190630224654928](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630224654928.png)

人们可以触摸并按住或双击文本字段，文本视图，Web视图或图像视图中的元素，以选择内容并显示编辑选项，例如复制和粘贴。

* 显示当前上下文的相应命令。

* 如有必要，调整编辑选项的位置。
* 不要使用与编辑菜单相同的功能实现其他控件。
* 允许选择和复制可能有用的不可编辑文本。
* 不要为按钮添加编辑选项。
* 使编辑操作无法撤消。
* 最小化自定义命令的数量。
* 保持自定义命令名称简短

### Page Controls-页面控件

![image-20190630224921903](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630224921903.png)

页面控件显示当前页面在平面页面列表中的位置。它显示为一系列小指示点，表示打开顺序中的可用页面。实心点表示当前页面。在视觉上，这些点总是等距的，并且如果在屏幕上出现太多则会被剪裁。用户可以点击页面控件的前沿或后端来访问下一页或上一页，但是他们无法点击特定点来转到特定页面。导航总是按顺序发生，通常是通过将页面滑动到一侧。

* 不要对具有分层页面的页面控件使用。
  * 页面控件不显示页面的相关性或指示哪个页面对应于每个点。此类控件设计用于彼此对等的页面。
* 不要显示太多页面。
  * 超过大约10个点很难一目了然，超过大约20个打开的页面按顺序访问是耗时的。
* 屏幕底部的中心页面控件。
  * 页面控件应始终居中并位于内容底部和屏幕底部之间。这使其保持可见，而不会阻止内容。

### Pickers-选择器

选择器包括一个或多个不同值的可滚动列表，每个值都具有单个选定值 - 出现在视图中心的较暗文本中。当用户编辑字段或点击菜单时，选取器通常显示在屏幕底部或弹出窗口中。选择器也可以显示为内联，例如在日历事件中编辑日期时。拾取器的高度大致是五行列表值的高度。拾取器的宽度可以是屏幕的宽度或其封闭视图，具体取决于设备和上下文。

![image-20190630225242699](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630225242699.png)

* 使用可预测和逻辑顺序的值。
  * 当可滚动列表静止时，可以隐藏选取器中的许多值。当人们可以预测这些值是什么时最好，例如使用按字母顺序排列的国家/地区列表，这样他们就可以快速浏览列表。
* 避免切换屏幕以显示选择器。
  * 当在正在编辑的字段下方或附近显示时，选取器工作良好。
* 对于大值列表，请使用表而不是选择器。
  * 长列表在选择器中导航可能很繁琐。一张桌子的高度可调，可以包含索引，滚动速度更快。

### Date Pickers-日期选择器

日期选择器是用于选择特定日期，时间或两者的有效界面。它还提供了一个显示倒数计时器的界面。

* 在指定分钟时考虑提供较少的粒度。

### Progress Indicators

不要让人们坐在静止的屏幕上等待你的应用程序加载内容或执行冗长的数据处理操作。使用活动指示器和进度条让人们知道您的应用程序没有停顿，并让他们知道他们将等待多长时间。

### Activity Indicators

当执行无法量化的任务（例如加载或同步复杂数据）时，活动指示符会旋转。任务完成后它会消失。活动指标是非交互性的。

![image-20190630225455152](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630225455152.png)

* 支持进度条超过活动指标。
  * 如果活动是可量化的，请使用进度条而不是活动指示器，以便人们可以更好地衡量正在发生的事情以及需要多长时间。
* 保持活动指标的移动。
  * 人们将固定活动指标与停滞过程联系起来。让它旋转，让他们知道正在发生的事情。
* 如果它有用，请在等待任务完成时提供有用的信息。
  * 在活动指标上方添加标签以提供额外的背景信息。避免使用模糊的术语，如加载或验证，因为它们通常不会添加任何值。

### Progress Bars-进度条

进度条包括从左到右填充的轨道，以显示具有已知持续时间的任务的进展。进度条是非交互式的，尽管它们通常伴有用于取消相应操作的按钮。

![image-20190630225608410](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630225608410.png)

* 始终准确报告进度。
  * 请勿显示不准确的进度信息，以使您的应用显示繁忙。仅对可量化的任务使用进度条。否则，请使用活动指示器。
* 对具有明确定义的持续时间的任务使用进度条。
  * 进度条非常适合显示任务的状态，特别是当它有助于传达任务需要完成的时间。
* 隐藏导航栏和工具栏中未填充的轨道部分。
* 考虑自定义进度条的外观以匹配您的应用。

### Network Activity Indicators

在没有边缘到边缘显示的设备上，网络活动指示器在网络发生时在屏幕顶部的状态栏中旋转。网络完成后它会消失。该指标看起来就像一个活动指标，并且是非交互式的。

![image-20190630225957214](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630225957214.png)

* 仅针对持续时间超过几秒的网络操作显示此指示器。
  * 不要显示快速网络操作的指示器，因为它可能会在任何人注意到它的存在之前消失或者意识到它的通信意味着什么。

### Refresh Content Controls-刷新内容控件

手动启动刷新控件以立即重新加载内容，通常在表视图中，而无需等待下一次自动内容更新发生。刷新控件是一种特殊类型的活动指示器，默认情况下是隐藏的，并且在向下拖动要重新加载的视图时变为可见。例如，在Mail中，您可以向下拖动收件箱邮件列表以检查新邮件。

![image-20190630230326138](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630230326138.png)

* 执行自动内容更新。
  * 虽然人们很欣赏能够立即触发内容刷新，但他们也希望定期进行自动刷新。不要让用户负责启动每个更新。定期更新数据，保持数据新鲜。
* 只有在增加价值时才提供简短标题。
  * 可选地，刷新控件可以包括标题。在大多数情况下，这是不必要的，因为控件的动画表明内容正在加载。如果您确实包含标题，请不要使用它来解释如何执行刷新。而是提供有关正在刷新的内容的有价值信息。例如，Podcast中的刷新控件使用标题告诉人们上次播客更新的时间。

### Segmented Controls-分段控件

分段控件是两个或更多个段的线性集合，每个段用作互斥按钮。在控件内，所有段的宽度相等。与按钮一样，细分可以包含文本或图像。分段控件通常用于显示不同的视图。

![image-20190630230551203](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630230551203.png)

* 限制段数以提高可用性。
  * 分段控件应该有五个或更少的段。
* 尽量保持段内容大小一致。
* 避免在分段控件中混合文本和图像。
* 将内容适当地放在自定义分段控件中。

### Steppers

步进器是用于增加或减少增量值的两段控制。默认情况下，步进器的一个段显示加号，另一个段显示减号。如果需要，可以用自定义图像替换这些符号。

![image-20190630230744208](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630230744208.png)

* 使步进器影响的值明显。
  * 步进器本身不显示任何值，因此请确保人们知道在使用步进器时它们正在改变哪个值。
* 当可能发生大的值变化时，请勿使用步进器。
  * 步进器可以很好地进行需要轻微敲击的小改动。例如，在打印屏幕上，使用步进器设置份数是有意义的，因为人们很少更改此设置。另一方面，使用步进器选择页面范围是没有意义的，因为即使合理的页面范围也需要大量的点击。

### Switches

开关是两个互斥状态 - 开和关之间的视觉切换。

![image-20190630230855507](/Users/huangsong/Library/Application Support/typora-user-images/image-20190630230855507.png)

* 考虑调整开关的外观以匹配您的应用程序的样式。
* 仅在表行中使用开关。
  * 开关用于表格，例如可以打开和关闭的设置列表。如果您需要工具栏或导航栏中的类似功能，请改用按钮，并提供两个不同的图标来传达状态。
* 避免添加标签来描述Switches的值。
  * 开关打开或关闭。提供描述这些状态的标签是多余的并且使界面混乱。
* 考虑使用开关来管理相关界面元素的可用性。








































































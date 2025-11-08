# YouTube Plus (ex. YTLite)

iOS 版 YouTube 用フレキシブルエンハンサー。100 以上のカスタマイズ可能なオプションを搭載。

## 目次

- [スクリーンショット](#スクリーンショット)
- [主な機能](#主な機能)
- [FAQ](#faq)
- [レビュー](#レビュー)
- [GitHub Actions を使用して Youtube Plus を構築する方法](#github-actions-を使用して-youtube-plus-を構築する方法)
- [サポートしているバージョン](#サポートしているバージョン)
- [お借りした機能](#お借りした機能)

## スクリーンショット

<table>
   <tr>
      <td><img src="Resources/scr1.jpg" alt="Screenshot 1" /></td>
      <td><img src="Resources/scr2.jpg" alt="Screenshot 2" /></td>
      <td><img src="Resources/scr3.jpg" alt="Screenshot 3" /></td>
   </tr>
</table>

<details>
  <summary>他のスクショ</summary>
  <table>
    <tr>
      <td><img src="Resources/scr4.jpg" alt="Screenshot 4" /></td>
      <td><img src="Resources/scr5.jpg" alt="Screenshot 5" /></td>
      <td><img src="Resources/scr6.jpg" alt="Screenshot 6" /></td>
    </tr>
    <tr>
      <td><img src="Resources/scr7.jpg" alt="Screenshot 7" /></td>
      <td><img src="Resources/scr8.jpg" alt="Screenshot 8" /></td>
      <td><img src="Resources/scr9.jpg" alt="Screenshot 9" /></td>
    </tr>
  </table>
</details>

## 主な機能

<li>動画・音声・サムネイル・ポスト投稿・プロフィール画像のダウンロード</li>
<li>動画概要欄・<a title="文字としてコピーだけじゃなく、画像としてもコピーできるし、保存もできるぞ！！">コメントのコピー</a></li>
<li>UIのカスタマイズ・タブの並び替え・ <a title="たとえば黒を表現する際、通常少し灰色っぽくなるが、OLEDだと完全な黒を再現することが出来ます。">OLEDモードの有効化</a></li>
<li>プレイヤー設定：ジェスチャー・<a title="Wi-Fi接続時とモバイルデータ使用時で、デフォルトにする画質を変更することが出来ます。">標準画質の設定</a>・<a title="閲覧する動画に、設定した言語が存在する場合のみ有効です。">優先オーディオトラック</a></li>
<li>Youtube PLUSの設定の保存・読み込み・初期化、キャッシュの手動・自動削除</li>
<li>SponsorBlockを搭載</li>
<li>その他の機能はご自身で試してみて！</li>
<br>

**YouTube Plus の設定は YouTube の設定画面で確認できます**

**すべての貢献者は「貢献者」セクションに記載されています**
**使用したオープンソースライブラリは「オープンソースライブラリ」セクションに記載されています**

## FAQ

<details>
  <summary>YouTube PlusはどのiOSバージョンに対応していますか？</summary>
    <p><br>YouTube PlusはiOS 14以降に対応しています。<strong>ですが、脱獄していないデバイスにインストールする場合は、YouTubeアプリとご利用のiOSバージョンの互換性も考慮する必要があります。</strong><br>以下がiOSごとにサポートされている最新のYouTubeバージョンのリストです。</p>
    <li><strong>iOS 14</strong>: YouTube v19.20.2</li>
    <li><strong>iOS 15</strong>: YouTube v20.21.6</li>
    <li><strong>iOS 16+</strong>: 全てのバージョンに対応</li>
</details>
<br>
<details>
  <summary>最新のYouTubeアプリで、私のiOSバージョンがサポートされなくなりました。どうすればよいですか？</summary>
    <p><br>いくつかの方法をご紹介します。</p>
    <li><a href="https://ios.cfw.guide/get-started/">デバイスを脱獄</a>し、 App Storeから対応しているYouTubeバージョンをインストールし、<a href="http://dvntm0.github.io/#jb">Tweakとしてインストール</a>してください。</li><br>
    <li><a href="https://ios.cfw.guide/installing-trollstore/">TrollStoreをインストール</a>し、次に <a href="https://github.com/Lessica/TrollFools/releases/">TrollFools</a>をインストールして、App Storeから対応しているYouTubeバージョンをインストールしたのち、TrollFoolsを使用して <a href="https://github.com/dayanch96/YTLite/releases/">YouTube Plus</a> を注入してください。</li><br>
    <li>互換性のあるIPAをオンラインで探し、 <a href="../README.md#github-actions-を使用して-youtube-plus-を構築する方法">GitHub Actionsを使用してYouTube Plusアプリを構築する</a></li>
</details>
<br>
<details>
  <summary>Cast stopped working on sideloaded YouTube Plus. What should I do?</summary>
    <p>Until this issue is resolved, it is recommended to use YouTube version 20.14.1 or below.</p>
</details>
<br>
<details>
  <summary>When I try to play a video, I get <strong><em>Something went wrong. Refresh and try again later.</em></strong></summary>
    <p>Before jumping to conclusions, let’s clarify a few things:</p>
    <ol>
      <li><strong>This is NOT</strong> caused by ad blocking</li>
      <li><strong>This is NOT</strong> because your account was magically flagged</li>
      <li><strong>This is NOT</strong> due to your account being secretly blacklisted</li>
    </ol>
    <br>
    <p>The issue seems to lie somewhere in the sideloading process itself, even without any tweaks applied. It might be related to an invalid or missing VisitorID or VisitorData, as suggested <a href="https://github.com/pepeloni-away/userscripts/issues/6#issuecomment-2860641610">here</a>. This error has become more frequent due to YouTube’s stricter anti-download measures.</p>
    <br>
    <p><strong>Possible temporary workaround:</strong></p>
    <ol>
      <li>Sign out of your current account (or all accounts) completely: Go to the <em>You tab → Switch account → Manage accounts on this device → Remove from this device</em></li>
      <li>Watch a few full-length videos without being signed in. Stay signed out for a few hours.</li>
      <li>Sign back into the account that was having issues</li>
    </ol>
</details>

## レビュー

Review by [@qbap](https://github.com/qbap) on ONE Jailbreak: https://onejailbreak.com/blog/youtube-plus/

## GitHub-Actions を使用して Youtube-Plus を構築する方法

> [!NOTE]
> If this your first time, complete following steps before starting:
>
> 1. Fork this repository using the fork button on the top right
> 2. On your forked repository, go to **Repository Settings** > **Actions**, enable **Read and Write** permissions.

<details>
  <summary>How to build the YouTube Plus app</summary>
  <ol>
    <li>Click on <strong>Sync fork</strong>, and if your branch is out-of-date, click on <strong>Update branch</strong>.</li>
    <li>Navigate to the <strong>Actions tab</strong> in your forked repository and select <strong>Build YouTube Plus app</strong>.</li>
    <li>Click the <strong>Run workflow</strong> button located on the right side.</li>
    <li>Mark or unmark the tweaks you want to integrate. Learn more about them in the <a href="#tweak-integration-details">Tweak Integration Details</a> section.</li>
    <li>Prepare a decrypted .ipa file <em>(we cannot provide this due to legal reasons)</em>, then upload it to a file provider (e.g., filebin.net, filemail.com, or Dropbox is recommended). Paste the URL of the decrypted IPA file in the provided field.</li>
    <li><strong>NOTE:</strong> Make sure to provide a direct download link to the file, not a link to a webpage. Otherwise, the process will fail.</li>
    <li>Enter the tweak version from the releases (the latest release is selected by default). You can also change the BundleID and Display Name if desired.</li>
    <li>Make sure all inputs are correct, then click <strong>Run workflow</strong> to start the process.</li>
    <li>Wait for the build to finish. You can download the YouTube Plus app from the releases section of your forked repo. (If you can't find the releases section, go to your forked repo and add /releases to the URL, i.e., github.com/user/YTLite/releases.)</li>
  </ol>
</details>

<details>
  <summary>How to build the YouTube Plus app with your own link for the YouTube Plus tweak</summary>
  <ol>
    <blockquote>
      <p><strong>NOTE:</strong> This option is primarily intended for building the YouTube Plus app based on the beta file you have. In other cases, it is generally not needed.</p>
    </blockquote>
    <li>Click on <strong>Sync fork</strong>, and if your branch is out-of-date, click on <strong>Update branch</strong>.</li>
    <li>Navigate to the <strong>Actions tab</strong> in your forked repository and select <strong>[BETA] Build YouTube Plus app</strong>.</li>
    <li>Click the <strong>Run workflow</strong> button located on the right side.</li>
    <li>Mark or unmark the tweaks you want to integrate. Learn more about them in the <a href="#tweak-integration-details">Tweak Integration Details</a> section.</li>
    <li>Prepare a decrypted .ipa file <em>(we cannot provide this due to legal reasons)</em>, then upload it to a file provider (e.g., filebin.net, filemail.com, or Dropbox is recommended). Paste the URL of the decrypted IPA file in the provided field.</li>
    <li>Upload your beta tweak file to a file provider and paste direct link to the <strong>URL to the YouTube Plus tweak file</strong> field. You can also change the BundleID and Display Name if desired.</li>
    <li><strong>NOTE:</strong> Make sure to provide a direct download link to the file, not a link to a webpage. Otherwise, the process will fail.</li>
    <li>Make sure all inputs are correct, then click <strong>Run workflow</strong> to start the process.</li>
    <li>Wait for the build to finish. You can download the YouTube Plus app from the releases section of your forked repo. (If you can't find the releases section, go to your forked repo and add /releases to the URL, i.e., github.com/user/YTLite/releases.)</li>
  </ol>
</details>

## サポートしているバージョン

<ul>
   <li><strong>Latest confirmed:</strong> <em>20.29.3</em></li>
   <li><strong>Date tested:</strong> <em>July 25, 2025</em></li>
   <li><strong>YouTube Plus:</strong> <em>5.2 beta 2</em></li>
</ul>

## お借りした機能

<details>
  <summary>YouPiP</summary>
  <p>YouPiP is a tweak developed by <a href="https://github.com/PoomSmart">PoomSmart</a> that enables the native Picture-in-Picture feature for videos in the iOS YouTube app.</p>
  <p><strong>YouPiP preferences</strong> are available in the <strong>YouTube settings</strong>.</p>
  <p>Source code and additional information are available <a href="https://github.com/PoomSmart/YouPiP">in PoomSmart's GitHub repository</a>.</p>
</details>

<details>
  <summary>YTUHD</summary>
  <p>YTUHD is a tweak developed by <a href="https://github.com/PoomSmart">PoomSmart</a> that unlocks 1440p (2K) and 2160p (4K) resolutions in the iOS YouTube app.</p>
  <p><strong>YTUHD preferences</strong> are available in the <strong>Video quality preferences</strong> section under <strong>YouTube settings</strong>.</p>
  <p>Source code and additional information are available <a href="https://github.com/PoomSmart/YTUHD">in PoomSmart's GitHub repository</a>.</p>
</details>

<details>
  <summary>Return YouTube Dislikes</summary>
  <p>Return YouTube Dislikes is a tweak developed by <a href="https://github.com/PoomSmart">PoomSmart</a> that brings back dislikes on the YouTube app.</p>
  <p><strong>Return YouTube Dislikes preferences</strong> are available in the <strong>YouTube settings</strong>.</p>
  <p>Source code and additional information are available <a href="https://github.com/PoomSmart/Return-YouTube-Dislikes">in PoomSmart's GitHub repository</a>.</p>
</details>

<details>
  <summary>YouQuality</summary>
  <p>YouQuality is a tweak developed by <a href="https://github.com/PoomSmart">PoomSmart</a> that allows to view and change video quality directly from the video overlay.</p>
  <p><strong>YouQuality can be enabled</strong> in the <strong>Video overlay</strong> section under <strong>YouTube settings</strong>.</p>
  <p>Source code and additional information are available <a href="https://github.com/PoomSmart/YouQuality">in PoomSmart's GitHub repository</a>.</p>
</details>

<details>
  <summary>DontEatMyContent</summary>
  <p>DontEatMyContent is a tweak developed by <a href="https://github.com/therealFoxster">therealFoxster</a> that prevents the Notch/Dynamic Island from munching on 2:1 video content in the iOS YouTube app.</p>
  <p><strong>DontEatMyContent preferences</strong> are available in the <strong>YouTube settings</strong>.</p>
  <p>Source code and additional information are available <a href="https://github.com/therealFoxster/DontEatMyContent">in therealFoxster's GitHub repository</a>.</p>
</details>

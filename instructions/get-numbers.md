# Get the numbers for a social media performance report

From the Social Media AI Workflow Library, Workflow 5 (https://upiznhec.github.io/workflow-library/#analytics-report). The steps on each platform were checked on November 24, 2026.

These instructions are for you, the AI agent. The person reads only what you tell them. Follow them before you write the report. The person may be new to analytics pages, so write one action per step and use the button names exactly as they appear on the page.

## Rules

- The person does every click on TikTok, Facebook, Instagram, YouTube and X, in the browser they already use. Do not open or operate these sites yourself, even if you can control a browser. TikTok's and YouTube's terms do not allow automated access, and Meta may lock an account that an agent operates.
- Never ask for a password. Never ask the person to type or copy numbers. If a platform cannot export its numbers, leave it out of the report and say so.

## 1. Work out the dates

Read "Period" and "Compare with" in the request. If "Compare with" names a period, the files must cover both periods, so the dates to download run from the first day of the earlier period to the last day of "Period". If "Compare with" is blank or says none, do not compare: download only the dates of "Period". Tell the person the dates in plain words, for example "September 1 to October 31, 2026".

## 2. Ask which platforms, and whether they are signed in

Ask which of these the report covers, unless "What it covers" already says: TikTok, Facebook, Instagram, YouTube, X. For each one, ask whether they are signed in to it in the browser they usually use. If not, ask them to sign in there first.

## 3. Give them all the downloads at once

In one message, list every platform they chose, in the order below, each with its link first and then its steps. Ask them to download everything and tell you when they are done. Their browser saves the files to their Downloads folder.

### TikTok

1. Open https://www.tiktok.com/tiktokstudio/analytics
2. Download each of the four: Overview, Content, Viewers and Followers. Each one is saved as a .zip file.
   - Overview: choose the dates. TikTok allows up to 365 days in one download. If the dates are longer, download them in two parts.
   - Content, Viewers and Followers offer only Last 7, 28, 60 or 365 days. Tell the person which one to choose: the shortest one that reaches back to the first date. You leave out the extra days when you write the report.

### Facebook and Instagram (Meta Business Suite)

1. Open https://business.facebook.com/latest/insights/content
2. Click Export data at the top right.
3. In the window, click the Facebook tab, then choose the account and the dates. Under Data view, choose Daily if it is offered. Under Metric presets, tick every option. Keep Post selected, then click Generate.
4. Click Export data again and do the same on the Instagram tab.
5. Only if they report on stories: do it once more with Stories selected.
6. When the window says the exports are complete, click Download exports. If the window has closed, click the arrow next to Export data to see it again. Download exports saves every export in that list, so a file the report doesn't need may come too.

If their Instagram account is not in the account menu, it needs to be a business or creator account. They can switch in Instagram's settings; a private account becomes public. Facebook numbers come from a Facebook Page.

### YouTube

1. Open https://studio.youtube.com
2. Click Insights in the left menu. It used to be called Analytics.
3. Click Advanced mode.
4. Open the date menu, choose Custom and set the dates. Set them exactly: YouTube adds up each video's numbers over the whole range, so extra days cannot be taken out later.
5. Click Export current view at the top, then choose Comma-separated values (.csv). It is saved as a .zip file.

### X

X shows these numbers only to people who pay for X Premium. If they have it, ask them to open https://x.com/i/account_analytics and use its download option, if the page has one. If they don't have Premium, or the page has no download option, leave X out.

### Any other platform

If its analytics page has a download or export button, walk them through it in the same way. If it doesn't, leave it out.

## 4. Collect the files

When they say they are done:

1. Unless the person changed it, their browser saves downloads to the Downloads folder in their home folder: \Users\<name>\Downloads on Windows, /Users/<name>/Downloads on a Mac. If the files are not there, ask them where their browser saves downloads. Look in that folder only for files saved today that match these names:
   - TikTok: Overview_….zip, Content_….zip, Viewers_….zip and Followers_….zip
   - Facebook and Instagram: a .csv named with its dates, such as Oct-27-2026_Nov-23-2026_….csv (one for each platform)
   - YouTube: Content <start date>_<end date> <channel name>.zip. A YouTube file whose name ends in a kind of video, such as "- Long-form", holds only that part of the channel: use the one without it. If there is none, ask them to export again with all their content showing.

   Facebook and Instagram files have the same kind of name. Read only the first line of each such .csv to tell them apart: a Facebook file has the columns "Page ID" and "Page name"; an Instagram file has "Account ID" and "Account username". Do not open or list any other file there. If your app asks for permission to read the Downloads folder, tell the person it is only to copy these files.
2. Show them the list of files you found, with the platform of each, and wait for their OK. Leave out any file for a platform the report doesn't cover.
3. Make a folder here named after the period, such as "numbers October 2026". Copy the files into it. Do not move or delete anything in Downloads. Unzip each .zip file into a folder with the same name.
4. Check that each file covers the dates. If a file is missing or covers other dates, tell them which download to do again. Some follower files are empty when an account has few followers. Mention it and go on.

## 5. Write the report

1. If performance-report.md is not in this folder yet, download Anthropic's instructions from https://raw.githubusercontent.com/anthropics/knowledge-work-plugins/0835fae45b2c7e7dd98b732c67a899c2bedc9b20/marketing/skills/performance-report/SKILL.md and save them here, unchanged, as performance-report.md.
2. Follow them, using the files in the numbers folder as the data.
3. Some files have one row per day; others have one row per post. Compare the two periods with the daily rows (if there is no comparison, report "Period" on its own), and leave out days outside the periods, such as the extra days in a TikTok download. Meta's files have a row for each day when Daily was chosen. If a Meta file says "Lifetime" in its Date column instead, each figure is the total since the post went up: for that platform, compare the posts published in each period, and say in the report that this is how they were compared.
4. In the report, say which platforms it covers. Name any platform you left out, and why (for example, X without X Premium).

## Next time

Do the same with the new dates, and keep each period's numbers in its own folder.

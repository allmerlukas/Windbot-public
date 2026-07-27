# Privacy Policy — Wind Bot

_Last updated: July 27, 2026_

This policy explains what data Wind Bot collects, why it collects it, and how it is stored and protected. Wind Bot does not sell, rent, or share your data with any third party for advertising or commercial purposes.

## 1. Who We Are

Wind Bot ("the Bot", "we", "our") is a Discord bot providing a partner Auto-Wave ad exchange, partner statistics and leaderboards, and related server tools. **This policy covers those features.** The DonutSMP Spawner Shop and its minigame giveaways are a separate, single-server feature with their own Privacy Policy — see `shop-privacy.md`. The Bot is operated by its developer ("Developer"). For contact information, see Section 10.

## 2. Data We Collect

Wind Bot only collects data that is necessary to provide its features:

- **Guild (server) IDs:** used for per-server configuration.
- **Channel and role IDs:** partner, ad, and log channels, and member and ping roles, used for Auto-Wave routing and setup.
- **User IDs and usernames:** the ad host and users who post partner links, used for Auto-Wave routing and partner tracking and leaderboards.
- **Ad message content:** the text in your configured ad channel, read only to send Auto-Wave partner ads.
- **Partner URLs:** server invite links, used for partner link tracking and deduplication.
- **Server member counts:** a server's member count at the time it receives a partner ad, and again roughly 24 hours later, used to measure whether receiving a given partner's ad is associated with real growth. This is aggregate, server-level data (member counts are already publicly visible on Discord); it does not identify or track any individual member.

Wind Bot does not read general chat across your server. It reads message content only in the specific ad channel you configure via `/config setup`.

## 3. Why We Collect It

All data collection is tied to a specific bot feature:

- **Guild, channel, and role IDs:** to route Auto-Wave partner ads in the correct channels.
- **User IDs and usernames:** to associate partner-link posts with the right people and to display partner statistics and leaderboards.
- **Partner URLs:** to deduplicate partner links and provide partnership statistics.
- **Server member counts:** to measure and improve Auto-Wave partner matching over time, favoring partners that are associated with real server growth.

## 4. Data Storage and Security

Data is stored in a Supabase (PostgreSQL) database, and the bot is hosted on Railway. Access to the database is restricted to the Developer via secret credentials that are never exposed publicly.

- The database is not publicly accessible.
- The bot does not handle or store any real-world payment or financial information.
- Access is protected by provider access controls and Row Level Security.

Your data is used only to operate Wind Bot's features. It is never sold or shared for advertising.

## 5. Data Retention

- **Guild configuration:** retained while the bot remains in your server. You may request deletion (see Section 7).
- **Partner links:** daily records are pruned after 30 days automatically.
- **Ad performance records:** member-count snapshots tied to a specific ad delivery, retained to keep partner-matching statistics accurate.
- **Error logs:** a rolling window of the most recent errors; older entries are deleted automatically.

## 6. Third Parties

Wind Bot relies on the following third-party services to function, and does not share your data with anyone else:

- **Discord API** (discord.com): required for the bot to operate. Discord's own privacy policy applies to data held by Discord.
- **Supabase:** hosts the database where the data described above is stored.
- **Railway:** hosts the bot's application.

We do not sell, rent, or share your data with any third party for advertising or commercial purposes.

## 7. Your Rights

You have the right to:

- **Access:** request a summary of what data is stored for your guild or user ID.
- **Deletion:** request that data associated with your guild or user ID be deleted, subject to records we must keep for dispute resolution or fraud prevention.
- **Correction:** update stored configuration via the bot's slash commands (for example, `/config setup`).

To exercise these rights, contact us via Section 10.

## 8. Children's Privacy

Wind Bot is not directed at children under the age of 13, and Discord's own Terms of Service require users to be at least 13 years old. We do not knowingly collect personal data from children under 13. Wind Bot's Auto-Wave and partner features do not involve any real-world money.

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the "Last updated" date at the top of this page. Continued use of the bot after changes constitutes acceptance of the revised policy.

## 10. Contact

For any privacy-related questions or data deletion requests, contact the bot developer on Discord: https://discord.com/users/1493273832432210042

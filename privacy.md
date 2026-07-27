# Privacy Policy — Wind Bot

_Last updated: July 27, 2026_

This policy explains what data Wind Bot collects, why it collects it, and how it is stored and protected. Wind Bot does not sell, rent, or share your data with any third party for advertising or commercial purposes.

## 1. Who We Are

Wind Bot ("the Bot", "we", "our") is a Discord bot providing a partner Auto-Wave ad exchange, partner statistics, the DonutSMP Spawner Shop (a ticket-based system for buying and selling in-game Minecraft spawners), and sponsor-funded minigame giveaways, along with related server tools. The Spawner Shop is available only inside one specific, official server operated by the Developer, so all shop and ticket data is collected from that single server and adding Wind Bot to another server does not enable the shop there. The Bot is operated by its developer ("Developer"). For contact information, see Section 10.

## 2. Data We Collect

Wind Bot only collects data that is necessary to provide its features:

- **Guild (server) IDs:** used for per-server configuration.
- **Channel and role IDs:** partner, ad, and log channels, and member, ping, and staff roles, used for Auto-Wave routing and shop and ticket setup.
- **User IDs and usernames:** ticket owner, buyer, seller, staff, and ad host, used for tickets, shop orders, staff payouts, and partner tracking.
- **Ad message content:** the text in your configured ad channel, read only to send Auto-Wave partner ads.
- **Partner URLs:** server invite links, used for partner link tracking and deduplication.
- **Shop transaction data:** spawner type, quantity, price, and buyer, seller, and staff IDs, used for orders, stock, sales statistics, staff payouts, and leaderboards.
- **Ticket transcripts:** messages sent inside a shop or support ticket, kept as a record of an order for dispute resolution.
- **Server member counts:** a server's member count at the time it receives a partner ad, and again roughly 24 hours later, used to measure whether receiving a given partner's ad is associated with real growth. This is aggregate, server-level data (member counts are already publicly visible on Discord); it does not identify or track any individual member.
- **Linked in-game names:** when you run `/link`, your DonutSMP in-game name (IGN) is stored and associated with your Discord user ID, so shop payments, giveaway entries, and prize payouts can be tied to a known account.
- **Payment-verification data:** for shop purchases and giveaway sponsorships, the expected amount, a small unique verification code added to that amount, and whether a matching payment was detected.
- **Minigame giveaway and sponsorship data:** which giveaways you joined, giveaways you hosted, your cumulative amount sponsored, winner and refund payout records, and your chosen sponsor cosmetic preferences (accent color, giveaway skin, banner emoji).
- **Public player statistics we look up:** to verify payments and validate an IGN, the Bot requests publicly-available player stats (such as in-game balance) from a third-party stats website (donutstats.net). See Section 6.

Wind Bot does not read general chat across your server. It reads message content only in the specific ad channel you configure via `/config setup`, inside shop and support ticket channels (which are saved as a transcript when the ticket closes), and, briefly during certain typed minigames (for example Type Racer and Unscramble), in the giveaway channel to detect the winning answer.

Public in-game names, Discord names, cumulative sponsorship totals, and giveaway results may be displayed publicly within the server (for example on leaderboards, giveaway posts, and sponsor announcements).

## 3. Why We Collect It

All data collection is tied to a specific bot feature:

- **Guild, channel, and role IDs:** to route Auto-Wave partner ads and to run the shop and ticket systems in the correct channels.
- **User IDs and usernames:** to associate tickets, orders, stock contributions, and staff payouts with the right people, and to display partner and sales statistics.
- **Partner URLs:** to deduplicate partner links and provide partnership statistics.
- **Shop transaction data:** to track stock, calculate what staff are owed, produce sales statistics and leaderboards, and reverse orders that are cancelled.
- **Ticket transcripts:** to keep a record of each order or support request in case of a dispute.
- **Server member counts:** to measure and improve Auto-Wave partner matching over time, favoring partners that are associated with real server growth.
- **Linked in-game names:** to tie shop payments, giveaway entries, and prize payouts to a known in-game account, and to know where to send a winner's prize.
- **Payment-verification and stats data:** to automatically confirm that an in-game payment was received before opening an order or posting a giveaway, and to validate that an IGN is a real player.
- **Giveaway and sponsorship data:** to run giveaways, determine winners, record who is owed a payout or refund, rank sponsors on leaderboards, assign sponsor tier roles, and apply your chosen cosmetic preferences.

## 4. Data Storage and Security

Data is stored in a Supabase (PostgreSQL) database, and the bot is hosted on Railway. Access to the database is restricted to the Developer via secret credentials that are never exposed publicly.

- The database is not publicly accessible.
- All shop payments are made in-game; the bot does not handle or store any real-world payment or financial information.
- Access is protected by provider access controls and Row Level Security.

Your data is used only to operate Wind Bot's features. It is never sold or shared for advertising.

## 5. Data Retention

- **Guild configuration:** retained while the bot remains in your server. You may request deletion (see Section 7).
- **Tickets:** the ticket channel is deleted when closed; a text transcript of shop and support tickets is retained for dispute resolution.
- **Shop records:** stock, sales, and payout records are retained to keep the shop's books accurate. Pending staff-payment entries are cleared once settled.
- **Partner links:** daily records are pruned after 30 days automatically.
- **Ad performance records:** member-count snapshots tied to a specific ad delivery, retained to keep partner-matching statistics accurate.
- **Linked in-game names:** retained until you re-link a different name or request deletion (see Section 7).
- **Giveaway, sponsorship, and payout records:** retained to run leaderboards, sponsor tiers, and keep an accurate record of prizes and refunds owed and paid.
- **Error logs:** a rolling window of the most recent errors; older entries are deleted automatically.

## 6. Third Parties

Wind Bot relies on the following third-party services to function, and does not share your data with anyone else:

- **Discord API** (discord.com): required for the bot to operate. Discord's own privacy policy applies to data held by Discord.
- **Supabase:** hosts the database where the data described above is stored.
- **Railway:** hosts the bot's application.
- **donutstats.net:** an independent, unofficial DonutSMP statistics website. To verify in-game payments and validate in-game names, the Bot requests publicly-available player stat pages from this site (for example an account's in-game balance). We only send an in-game name in the lookup; we do not send your Discord data to it. donutstats.net is operated by a third party we do not control, and its own terms and privacy practices apply to how it handles those requests. The Bot uses it on a best-effort basis and does not rely on it holding any of your data.

We do not sell, rent, or share your data with any third party for advertising or commercial purposes.

## 7. Your Rights

You have the right to:

- **Access:** request a summary of what data is stored for your guild or user ID.
- **Deletion:** request that data associated with your guild or user ID be deleted, subject to records we must keep for dispute resolution or fraud prevention.
- **Correction:** update stored configuration via the bot's slash commands (for example, `/config setup`).

To exercise these rights, contact us via Section 10.

## 8. Children's Privacy

Wind Bot is not directed at children under the age of 13, and Discord's own Terms of Service require users to be at least 13 years old. We do not knowingly collect personal data from children under 13. All Spawner Shop trading takes place in-game using DonutSMP's in-game currency; no real-world money is involved.

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the "Last updated" date at the top of this page. Continued use of the bot after changes constitutes acceptance of the revised policy.

## 10. Contact

For any privacy-related questions or data deletion requests, contact the bot developer on Discord: https://discord.com/users/1493273832432210042

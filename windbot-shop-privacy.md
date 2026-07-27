# Privacy Policy — DonutSMP Spawner Shop (Wind Bot)

> **Note regarding platform compliance:** The features described here (the Spawner Shop and its minigame giveaways) are a custom system operated inside a single Discord server, using DonutSMP in-game currency only, with no real-world money involved. If Discord, or any platform on which this is reviewed, does not accept this custom feature, please contact the developer (see Section 11) and the developer will promptly remove these features and, if required, delete the server.

_Last updated: July 27, 2026_

This policy explains what data the **DonutSMP Spawner Shop** and its **minigame giveaways** collect, why, and how it is stored and protected. These features are part of Wind Bot but run only inside one specific, official Discord server operated by the Developer; adding Wind Bot to another server does not enable them. The rest of Wind Bot (the Auto-Wave partner system and partner statistics) is covered by a separate Privacy Policy.

We do not sell, rent, or share your data with any third party for advertising or commercial purposes.

## 1. Scope

This policy applies to the Spawner Shop (a ticket-based system for buying and selling in-game Minecraft spawners on DonutSMP) and the sponsor-funded minigame giveaways (raffles and skill games, with sponsor tiers, perks, and leaderboards). It applies only within the single, official server where these features are offered. The Bot is operated by its developer ("Developer"); see Section 11 for contact.

## 2. Data We Collect

We only collect what is needed to run the shop and giveaways:

- **User IDs and usernames:** ticket owner, buyer, seller, staff, giveaway host, entrant, and winner, used for tickets, orders, payouts, giveaways, and leaderboards.
- **Linked in-game names (IGNs):** when you run `/link`, your DonutSMP in-game name is stored and associated with your Discord user ID, so payments, giveaway entries, and prize payouts can be tied to a known account.
- **Shop transaction data:** spawner type, quantity, price, and buyer, seller, and staff IDs, used for orders, stock, sales statistics, staff payouts, and leaderboards.
- **Ticket transcripts:** messages sent inside a shop or support ticket, kept as a record of an order for dispute resolution.
- **Payment-verification data:** the expected amount, a small unique verification code added to that amount, and whether a matching payment was detected.
- **Minigame giveaway and sponsorship data:** which giveaways you joined, giveaways you hosted, your cumulative amount sponsored, winner and refund payout records, and your chosen sponsor cosmetic preferences (accent color, giveaway skin, banner emoji).
- **Public player statistics we look up:** to verify payments and validate an IGN, the Bot requests publicly-available player stats (such as an in-game balance) from a third-party stats website (donutstats.net). See Section 6.

The Bot reads message content only inside shop and support ticket channels (saved as a transcript when the ticket closes) and, briefly during certain typed minigames (for example Type Racer and Unscramble), in the giveaway channel to detect the winning answer. It does not read general chat.

## 3. Why We Collect It

All collection is tied to a specific feature:

- **User IDs and usernames:** to associate tickets, orders, staff payouts, giveaway entries, and prizes with the right people.
- **Linked IGNs:** to tie payments and prizes to a known in-game account and to know where to send a winner's prize.
- **Shop transaction data:** to track stock, calculate what staff are owed, produce sales statistics and leaderboards, and reverse cancelled orders.
- **Ticket transcripts:** to keep a record of each order or support request in case of a dispute.
- **Payment-verification and stats data:** to automatically confirm that an in-game payment was received before opening an order or posting a giveaway, and to validate that an IGN is a real player.
- **Giveaway and sponsorship data:** to run giveaways, determine winners, record who is owed a payout or refund, rank sponsors on leaderboards, assign sponsor tier roles, and apply your cosmetic preferences.

## 4. Data Storage and Security

Data is stored in a Supabase (PostgreSQL) database, and the Bot is hosted on Railway. Access is restricted to the Developer via secret credentials that are never exposed publicly.

- The database is not publicly accessible, and is protected by provider access controls and Row Level Security.
- All shop and giveaway payments are made in-game; the Bot does not handle or store any real-world payment or financial information.

Your data is used only to operate these features. It is never sold or shared for advertising.

## 5. Data Retention

- **Linked IGNs:** retained until you re-link a different name or request deletion (see Section 8).
- **Tickets:** the ticket channel is deleted when closed; a text transcript is retained for dispute resolution.
- **Shop records:** stock, sales, and payout records are retained to keep the shop's books accurate. Pending staff-payment entries are cleared once settled.
- **Giveaway, sponsorship, and payout records:** retained to run leaderboards and sponsor tiers and to keep an accurate record of prizes and refunds owed and paid.
- **Error logs:** a rolling window of the most recent errors; older entries are deleted automatically.

## 6. Third Parties

- **Discord API** (discord.com): required for the Bot to operate. Discord's own privacy policy applies.
- **Supabase:** hosts the database.
- **Railway:** hosts the Bot's application.
- **donutstats.net:** an independent, unofficial DonutSMP statistics website. To verify in-game payments and validate in-game names, the Bot requests publicly-available player stat pages from this site (for example an account's in-game balance). We only send an in-game name in the lookup; we do not send your Discord data to it. donutstats.net is operated by a third party we do not control, and its own terms and privacy practices apply. The Bot uses it on a best-effort basis and does not rely on it holding any of your data.

We do not sell, rent, or share your data with any third party for advertising or commercial purposes.

## 7. Public Display

In-game names, Discord names, cumulative sponsorship totals, and giveaway results may be displayed publicly within the server, for example on shop and sponsor leaderboards, giveaway posts, and sponsor tier announcements. Member counts and other publicly-visible Discord information remain subject to Discord's own visibility settings.

## 8. Your Rights

You have the right to:

- **Access:** request a summary of what data is stored for your user ID.
- **Deletion:** request that data associated with your user ID be deleted, subject to records we must keep for dispute resolution or fraud prevention.
- **Correction:** update stored information via the Bot's slash commands (for example `/link`).

To exercise these rights, contact us via Section 11.

## 9. Children's Privacy

These features are not directed at children under 13, and Discord's Terms of Service require users to be at least 13. We do not knowingly collect personal data from children under 13. All shop and giveaway activity uses DonutSMP's in-game currency; no real-world money is involved.

## 10. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the "Last updated" date at the top. Continued use after changes constitutes acceptance of the revised policy.

## 11. Contact

For any privacy-related questions or data deletion requests, contact the Bot developer on Discord: https://discord.com/users/1493273832432210042

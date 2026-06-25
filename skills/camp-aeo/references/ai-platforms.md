# How each AI engine picks a camp, and how to let it in

Load this for the full-build tier, or when deciding which engines to prioritize. Every engine shares three baseline requirements: your camp must be in its index, crawlable by its bot, and extractable (it pulls passages, not pages). Beyond that, each weights different signals.

For a local camp, prioritize in this order, because that is where parents and the easiest wins are: Google AI Overviews and Gemini first, then ChatGPT, then Perplexity. Copilot and Claude are lower priority unless a specific audience uses them.

## Google AI Overviews and Gemini

Both lean on Google. Gemini is grounded directly in Google Maps and the Google index, and AI Overviews pull from the index with heavy weight on E-E-A-T (experience, expertise, authoritativeness, trustworthiness) and structured data.

What this means for a camp: the camp-seo work feeds these engines directly. A complete, accurate, verified Google Business Profile is the single biggest lever for Gemini, and strong reviews, schema, and trust signals feed AI Overviews. Notably, AI Overviews do not just recycle the top organic results, so a well-structured page can be cited even if it is not ranking first.

Focus: accurate Business Profile, schema markup, cited and accurate facts, real accreditation and staff credentials, content that answers parent questions.

## ChatGPT

Searches a Bing-based index and cites the web sources it used, leaning on third-party mentions and recent content. Domain authority and freshness matter, and content that reads the way ChatGPT would answer the question gets cited more.

Focus: be present and accurate on third-party sites parents trust (ACA listing, directories, reviews), keep pages current, and write direct, well-organized answers. Submit the site to Bing Webmaster Tools, not only Google.

## Perplexity

Always cites sources, runs results through quality reranking, and evaluates fresh content quickly. It has clear preferences:

- FAQ structured data (JSON-LD) gets cited noticeably more.
- Self-contained paragraphs it can lift cleanly.
- Publishing and updating regularly (freshness is a top factor).

Focus: FAQ content with schema, atomic answer passages, visible update dates.

## Copilot and Claude

- **Copilot** runs on Bing, so Bing indexing and page speed under two seconds help, plus presence on LinkedIn. Lower priority for most camps.
- **Claude** uses Brave Search when web search is enabled and is highly selective, favoring factually precise, well-sourced content. Confirm the camp shows in Brave Search, and keep facts specific and dated.

## Let the AI crawlers in

If `robots.txt` blocks an AI bot, that engine cannot cite the camp. Allow these user agents:

```
User-agent: GPTBot           # OpenAI, powers ChatGPT search
User-agent: ChatGPT-User     # ChatGPT browsing
User-agent: PerplexityBot    # Perplexity
User-agent: ClaudeBot        # Anthropic Claude
User-agent: anthropic-ai     # Anthropic Claude (alternate)
User-agent: Google-Extended  # Google Gemini and AI Overviews
User-agent: Bingbot          # Microsoft Copilot, via Bing
Allow: /
```

Some bots are used for both training and search citation. If a camp wants citation but not training use, the options are limited, since some bots do both. You can safely block CCBot (Common Crawl, training only) without losing any AI-search citations.

## Actions that help on every engine

1. Allow the AI crawlers above.
2. Keep the camp's core facts identical across the site, Google Business Profile, and directories.
3. Add schema (LocalBusiness, Course, Event, FAQPage).
4. Earn genuine, recent, well-rated reviews.
5. Answer real parent questions in clear, self-contained passages.
6. Show update dates and refresh content each season.

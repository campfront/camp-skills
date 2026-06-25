# Schema (JSON-LD) examples for a camp

Load this for the full-build tier, when adding structured data to camp pages. JSON-LD is the format Google recommends. Place it in the page `<head>` or at the end of `<body>`.

Three rules that matter more than the syntax:

1. **Accuracy**: mark up only what is genuinely on the page. False or padded markup earns no rich results and erodes trust.
2. **Completeness**: include the required properties for a type, or it does nothing.
3. **Validate**: test every block in the Rich Results Test (https://search.google.com/test/rich-results) before shipping, and watch the Search Console enhancement reports after.

Replace the placeholder values. Dates are ISO-8601 with a time-zone offset.

## LocalBusiness (homepage or contact page)

The base type for local results. For a day camp you can use the more specific `ChildCare`; `LocalBusiness` is the safe default.

```json
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "Camp Wildwood",
  "url": "https://campwildwood.com",
  "telephone": "+1-303-555-0123",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "123 Pine Trail",
    "addressLocality": "Denver",
    "addressRegion": "CO",
    "postalCode": "80202",
    "addressCountry": "US"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": 39.7392,
    "longitude": -104.9903
  },
  "openingHoursSpecification": [
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
      "opens": "08:00",
      "closes": "16:00"
    }
  ],
  "image": "https://campwildwood.com/photos/field.jpg",
  "sameAs": [
    "https://www.facebook.com/campwildwood",
    "https://www.instagram.com/campwildwood"
  ]
}
```

## Course (program page)

Use on each program page to describe the offering.

```json
{
  "@context": "https://schema.org",
  "@type": "Course",
  "name": "Soccer Day Camp in Denver, Ages 6-12",
  "description": "A week of skills, games, and small-sided matches for ages 6 to 12 in central Denver.",
  "provider": {
    "@type": "Organization",
    "name": "Camp Wildwood",
    "url": "https://campwildwood.com"
  }
}
```

## Event (a dated session or open house)

Use for each session with real dates. Repeat per session.

```json
{
  "@context": "https://schema.org",
  "@type": "Event",
  "name": "Soccer Day Camp Week 1",
  "startDate": "2026-06-15T09:00:00-06:00",
  "endDate": "2026-06-19T16:00:00-06:00",
  "eventStatus": "https://schema.org/EventScheduled",
  "eventAttendanceMode": "https://schema.org/OfflineEventAttendanceMode",
  "location": {
    "@type": "Place",
    "name": "Camp Wildwood",
    "address": {
      "@type": "PostalAddress",
      "streetAddress": "123 Pine Trail",
      "addressLocality": "Denver",
      "addressRegion": "CO",
      "postalCode": "80202",
      "addressCountry": "US"
    }
  },
  "organizer": {
    "@type": "Organization",
    "name": "Camp Wildwood",
    "url": "https://campwildwood.com"
  },
  "offers": {
    "@type": "Offer",
    "url": "https://campwildwood.com/programs/soccer-day-camp-denver/",
    "price": "295",
    "priceCurrency": "USD",
    "availability": "https://schema.org/InStock",
    "validFrom": "2026-01-05T00:00:00-07:00"
  }
}
```

## BreadcrumbList (any page with breadcrumbs)

```json
{
  "@context": "https://schema.org",
  "@type": "BreadcrumbList",
  "itemListElement": [
    { "@type": "ListItem", "position": 1, "name": "Home", "item": "https://campwildwood.com" },
    { "@type": "ListItem", "position": 2, "name": "Programs", "item": "https://campwildwood.com/programs/" },
    { "@type": "ListItem", "position": 3, "name": "Soccer Day Camp in Denver" }
  ]
}
```

## Combining types on one page (@graph)

A program page can carry several types at once. Wrap them in `@graph` rather than adding separate script tags.

```json
{
  "@context": "https://schema.org",
  "@graph": [
    { "@type": "Course", "name": "Soccer Day Camp in Denver, Ages 6-12", "provider": { "@type": "Organization", "name": "Camp Wildwood" } },
    { "@type": "BreadcrumbList", "itemListElement": [
      { "@type": "ListItem", "position": 1, "name": "Home", "item": "https://campwildwood.com" },
      { "@type": "ListItem", "position": 2, "name": "Programs", "item": "https://campwildwood.com/programs/" },
      { "@type": "ListItem", "position": 3, "name": "Soccer Day Camp in Denver" }
    ] }
  ]
}
```

## Do not bother with

- **FAQPage** for rich results: FAQ rich results no longer appear in Google Search (since May 2026). FAQ content can still help with AI assistants, which is camp-aeo's job, not this one.

# Data dictionary

File: `ai-search-observations-2026-10-15.csv`. UTF-8 CSV with a header and 14 data rows. Values are quoted. A reader should tolerate a UTF-8 byte-order mark.

| Column | Meaning | Values or format |
| --- | --- | --- |
| `query` | Exact search phrase used for this observation | Unicode text; English or Turkish |
| `market` | Country setting used for the search | `us` or `tr` |
| `language` | Requested language setting | `en` or `tr`; not a detected language label for every linked page |
| `observed_at_utc` | Recorded observation timestamp in UTC | `YYYY-MM-DD HH:mm:ss +00:00` |
| `device` | Device setting | `desktop` in this snapshot |
| `location_scope` | Geographic precision of the query setting | `country`; no city-level observation is implied |
| `ai_overview_count` | Number of AI Overview items recorded for this query capture | Integer; `1` for every row in this snapshot |
| `cited_urls` | Recorded source links extracted from the returned AI answer | Absolute URLs separated by ` | ` within one CSV cell |

One row is one query capture, not one cited page or one user. Expand `cited_urls` only when counting link records. Repeated URLs across rows remain repeated source occurrences.

No search-volume, ranking-difficulty, visitor, revenue, sentiment or platform-wide visibility column exists. A missing value in another study should not be converted to zero without an explicit definition. The present 14 rows are successful captures and do not describe the frequency of failed requests.

For joins, retain the full observation timestamp and the query settings. Query text alone is not a durable identifier once later dates are added.

Türkçe: Her satır bir sorgu gözlemidir. Bir hücrede birden çok kaynak URL’si bulunabilir. `market` ülkeyi, `language` istenen dili belirtir; kaynak sayfanın dili veya arayan kişinin uyruğu anlamına gelmez. Bu dosyada şehir, ziyaretçi, gelir veya özel hesap verisi yoktur.

# Methodology

Observation date: **2026-10-15**. Documentation prepared: **2026-10-19**.

## Research question

Which source links appeared in Google AI Overviews for a selected set of small-business questions, and what do the examples suggest about useful page content?

The panel was chosen for the questions a business owner might ask about website costs, local visibility, service websites and AI recommendations. It was not randomly sampled or weighted to represent national search demand.

## Collection

Fourteen Google searches were obtained through DataForSEO between **06:22:22 and 06:24:18 UTC**. Nine used the US/English setting; five used Turkey/Turkish. Device was desktop, with country-level location settings. The language field records the query setting, not the language of every cited page.

The public file preserves each query, market, language, observation time, device, location scope, Overview count and recorded source URLs. Source links came from numbered links in the returned answer text. Ordinary organic-result links were not added to this field. The report also discusses selected linked pages; it does not claim that every linked page was fully audited.

The CSV is the sanitized public record. Account details, task identifiers, full provider responses, complete generated answers and private site analytics are not included.

## Counting

Each CSV row is one query observation. Split `cited_urls` on the literal separator ` | ` to obtain link records. Count all occurrences to obtain **126** records. Count distinct full recorded URL strings to obtain **125**. For the hostname count, parse each URL, lowercase the hostname and remove a leading `www.`; the result is **100** hostnames.

Other subdomains remain distinct. A hostname is not a registrable-domain calculation, and a link record is not a unique domain. Query strings, timestamp fragments in video links and recorded redirect URLs are preserved. Redirect destinations were not exhaustively resolved. Different URLs that later lead to the same page may therefore remain separate records.

All 14 rows have `ai_overview_count = 1`. This is the result in the selected captures, not a general trigger rate. Counts describe recorded links, not visual prominence, citation share or a ranking of source quality.

## Interpretation

Questions about cost, business visibility and design produced different source mixes in the captured examples. The report uses that observation to suggest page improvements, including clear scope comparisons and working design examples. It does not identify proven ranking factors.

The two ChatGPT-related queries were searches on Google. There were no ChatGPT answer tests in this dataset. The panel does not cover AI Mode, mobile or named-city results. It does not measure clicks, leads, sales or the effect of subsequent edits.

## Repeating the study

Preserve this snapshot. Add later observations as a separately dated file with the same queries and recorded settings. Record missing or failed captures separately from successful answers without a source link. Compare source URLs and page content alongside any independently measured visits or inquiries. Do not overwrite the original date or treat a changed answer as proof that a page edit caused it.

## Türkçe yöntem özeti

Seçilmiş 14 sorgu, 15 Ekim 2026’da DataForSEO üzerinden ülke düzeyinde ve masaüstü ayarıyla alındı. Kaynak alanı, dönen AI yanıtındaki numaralı bağlantıları kaydeder; normal organik sonuçlar bu sayıya katılmaz. Kaynakların sınıflandırılması ve içerik önerileri yazarın değerlendirmesidir.

126 sayıma aynı bağlantının farklı sorgulardaki tekrarları dahildir. Farklı URL metinlerinin sayısı 125, www çıkarılmış hostname sayısı 100’dür. Çalışma tek tarihli örneklemdir; bütün pazarı, şehirleri, ChatGPT yanıtlarını veya yayın sonrası ticari gelişimi ölçmez.

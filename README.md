# CeneoScraper
## Selektory CSS składowych opinii w serwisie Ceneo.pl

| Składowa | Nazwa | Selektor |
| --- | --- | --- |
| Opinia | opinion/single opinion | div.js\_product-review |
| Identyfikator opinii | opinion\_id | [data-entry-id] |
| Autor | author | span.user-post\_\_author-name |
| rekomendacja | recommendation | span.user-post\_\_author-recommendation \> em |
| Liczba gwiazdek | score | span.user-post\_\_score |
| Czy opinia jest potwierdzona zakupem | purchased | div.review-pz |
| Data wystawienia opinii | opinion\_date | span.user-post\_\_published \> time:nth-child(1)[datetime] |
| Data zakupu produktu | purchase\_date | span.user-post\_\_published \> time:nth-child(2)[datetime] |
| Ile osób uznało opinię za przydatną | likes | button.vote-yes \> spanbutton.vote-yes[data-total-vote] |
| Ile osób uznało opinię za nieprzydatną | dislikes | button.vote-no \> spanbutton.vote-no[data-total-vote] |
| Treść opinii | content | div.user-post\_\_text |
| Listę wad | cons | div.review-feature\_\_title—negatives ~ div.review-feature\_\_item |
| Listę zalet | pros | div.review-feature\_\_title—positives ~ div.review-feature\_\_item |

## Wykorzystane biblioteki
    -Requests
    -BeautifulSoup
    -Os
    -Json
    -Pandas
    -Matplotlib
    -numpy
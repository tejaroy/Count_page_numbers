import re

PAGE_COUNT_REGEX = re.compile(rb"/Type\s*/Page([^s]|$)", re.MULTILINE | re.DOTALL)


def get_page_count(floc, regex=PAGE_COUNT_REGEX):
    """Count number of pages in a pdf"""
    with open(floc, "rb") as f:
        print(len(regex.findall(f.read())))


get_page_count(
    "C:/Users/TEJA/Downloads/00002_000009475_21072022_101430_loan_agreement_signedFinal_20220818124126 (1).pdf")
from PyPDF2 import PdfReader

reader = PdfReader("")
number_of_pages = len(reader.pages)
print(number_of_pages)


def get_page_count(floc):
    pdf_reader = PdfReader(floc)
    pages = len(pdf_reader.pages)
    return pages

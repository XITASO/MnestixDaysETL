1. Important Notice & Disclaimer 
Please read the following statements carefully before using the Mnestix ETL Demonstrator:
•This demonstration software is provided strictly for educational and testing purposes; it is not designed for production use.
•Depending on the DPP (Digital Product Passport) infrastructure (API) to which you upload data, your data may become publicly visible.
•If the chosen infrastructure is a test or publicly shared environment, it is possible that your data or the environment itself could be removed or altered at any time without prior notice.
•The software is provided AS IS, without warranty of any kind, under the terms of the MIT License. Please see Chapter 5 for the full license text.
 
2. How to Use the App 
Below is a quick guide to operating the Mnestix ETL Demonstrator:
•Select Excel File to choose your .xlsx or .xls.
•Then click Load Data to read and validate your Excel content.
•To refresh submodel definitions from Mnestix, click Load Submodels.
•Finally, create Digital Product Passports (DPPs) by clicking Save DPP.
 
3. Screens Explained 
The application provides several key screens:
•Main Screen: Houses buttons for loading submodels, selecting/loading Excel data, and saving DPPs.
•Products View: Displays loaded products in a tree structure. Each product node shows ID, Name, Type. Submodel nodes list fields and values. Invalid rows are highlighted or skipped.
•Templates View: Shows the submodel templates retrieved from Mnestix, including their name (displayName) and ID, plus mapping variables used to create a DPP.
 
4. Excel File Format Explained 
For successful data loading and DPP creation, structure your Excel file as follows:
•Products Worksheet:
- Columns ID, Name, Type are mandatory.
- Each row defines a unique product.
•Submodel Worksheets (e.g., Mechanics, Electronics):
- Must have columns ID (matching the Products sheet) and Template.
- Additional columns hold submodel variables.
•Validation:
- Any submodel row with unknown ID or missing Template is skipped.
- The Products sheet is mandatory or the file is invalid.
•Example Layout:
Products
| ID | Name         | Type      |
| P1 | Product One  | Physical  |
| P2 | Product Two  | Virtual   |
 
Submodel (Mechanics)
| ID | Template  | Length | Width |
| P1 | TemplateA | 100    | 50    |
| P2 | TemplateA | 200    | 80    |
| P3 | TemplateB | 150    | 60    |
 
5. MIT License 
The following license applies to this software:
MIT License
 
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
 
The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
 
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

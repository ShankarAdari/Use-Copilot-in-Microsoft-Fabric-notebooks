 We use Copilot for Fabric Data Engineering to load, transform, and save data in a Lakehouse. Let's imagine Contoso Health, a multi-specialty hospital network, wants to expand its services in the EU and wants to analyze projected population data.
 
 Source: EUROPOP2023 Population on January 1 by age, sex, and type of projection [proj_23np], Last updated June 28, 2023.

 Load data
Begin in a fresh notebook that's attached to your Lakehouse. In a new cell, you might try the following prompt. Prefixing with %%code signals to Copilot that you'd like generated code. Run it whenever you're ready to see what Copilot proposes.
(Run Copilot prompt to Load data)

Copilot generates code, which might differ slightly depending on your environment and the latest updates to Copilot.
(Run Python of Load data)

After running the cell, you should find the file downloaded and placed in the temporary folder of your Lakehouse.

In another new cell, you could ask Copilot to load the data like this:
(Run Copilot prompt2 to load data)

The resulting dataframe will contain the contents of the TSV file. One possible generated script could look like:
(Run Python2 file of Load data)

Transform data
Next, consider transforming the data: splitting the combined first field into separate columns, cleaning up unused fields, standardizing data types, and applying a bit of filtering. A prompt like the following in a new cell can guide Copilot:
(Run Colpilot prompt of Transform data)

Copilot generates code, which might differ slightly depending on your environment and the latest updates to Copilot.
(Run Python file of Transform data)

Save data
With transformations in place, you may want to persist the result to the Lakehouse. For instance, a cell prompt like this will have Copilot generate save logic:
(Run Copilot prompt of Save data)

Copilot generates code, which might differ slightly depending on your environment and the latest updates to Copilot.
(Run Python file of Save data)

Validation
To check that the table saved as expected, expand the Tables list in your Lakehouse and review its contents. You can also turn to the Copilot chat panel for quick exploratory questions; Copilot will reply with explanations or runnable code. 

For example:

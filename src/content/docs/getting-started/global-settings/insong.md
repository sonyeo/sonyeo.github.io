---
title: Features Overview
description: Welcome to your documentation site
---

import Grid from "~/components/user-components/Grid.astro";
import NewCard from "~/components/user-components/NewCard.astro";
import Button from "~/components/user-components/Button.astro";
import Accordion from "~/components/user-components/Accordion.astro";

# Features Overview

<Grid columns={3}>
  <NewCard title="Fast Setup" icon="rocket">
    Get started in minutes with our pre-configured setup
  </NewCard>

{" "}
<NewCard title="Custom Components" icon="document">
  Rich set of components for beautiful documentation
</NewCard>

  <NewCard title="Multilingual" icon="setting">
    Built-in support for multiple languages
  </NewCard>
</Grid>

<Accordion
  question="How do I add more pages?"
  answer="Simply create new .md or .mdx files in the src/content/docs/ directory"
/>

<Button
  label="View Full Documentation"
  link="/docs/components/using-components"
  variant="primary"
/>
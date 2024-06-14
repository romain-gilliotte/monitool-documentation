# Recommended order

When creating a project in Monitool, you may be tempted to start with the data sources, and then move on to the logical frameworks.

While this approach certainly works if you already have a clear idea of the whole monitoring and evaluation system of your project, it is not the most efficient way to get started and build as you go.

You may find yourself collecting data that you don't need, or need to refactor your project structure as you refine your logical framework.

The recommended order for setting up a project in Monitool is as follows

## 1. Basic information and sites

Start by entering the [basic information](./basic-information.md) of your project, such as the name, description, and then [the sites](./site.md) where the project will be implemented.

This is quick and usually requires little to no planning.

## 2. Logical framework

Build your [logical framework](./logical-framework.md) without worrying about the indicators or data sources that will be used to measure the progress of your project yet.

This is the most important part of your project, and it is where you should spend most of your time planning and thinking.

Iterate as many times as needed

## 3. Indicators

Once you are satisfied with the structure of your logical framework, [add the indicators](./indicators.md) that will be used to measure the progress of your project without worrying about how they will be computed.

When adding an indicator, you will be asked to select a computation method. Leave the default value `It is not possible to compute this indicator` for now, as you will add the data sources later.

## 4. Computing your first indicator

Start with a single indicator, and decide how you will collect the data to compute it.

The question you should ask yourself is:

- "What data do I need to collect to compute this indicator?"
- "Where can I find this data?"
- "Who will be responsible for collecting this data?"

In the case that you can't answer these questions, don't hesitate to go back to the logical framework and refine it.

### 4.1. Create the data source(s) for that indicator

Once you have answered these questions, you are ready to [create the data sources](./data-source.md) that will be used to collect the data needed to compute this particular indicator.

For example, if you are measuring the number of people that have been trained, you may need to create a data source for the training reports from your field staff.

If you are measuring the rate of antenatal consultations in a community, you may need to create two different data sources

- One for the health information system of the local health center, to collect the number of antenatal consultations.
- A second one for the surveys that will be conducted in the community to collect the number of expected pregnancies per month.

Most indicators will only require one data source, but some may require more than one.

### 4.2. Create invitations

Assigning each data source to the people responsible for collecting and entering the data is a crucial step.

This is done by creating [user invitations](./invite-other-users.md) as you go.

When assigning a data source to a user, you are doing two things at once:

- Documenting who is responsible for collecting the data
- Ensuring users will have access to the right sections in the data-entry interface

### 4.3. Update the indicator definition

Once you have created the data sources, you can go back to the indicator and update its definition to include the data sources that will be used to compute it.

## 5. Computing the next indicators

Repeat the process for the next indicators, one by one.

You will find that some indicators will require the same data sources, and that you can reuse them across different indicators.

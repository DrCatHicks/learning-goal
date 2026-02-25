# Learning Goal: A Claude Code Skill for Structured Goal Setting with Mental Contrasting

This skill guides you through a structured, interactive goal-setting exercise grounded in Mental Contrasting with Implementation Intentions (MCII), a self-regulation strategy supported by meta-analytic evidence that when used as a psychological intervention, this exercise can improve goal commitment and follow-through, decrease stress, and increase engagement and motivation. The exercise takes about 10-15 minutes and produces a concrete goal card you can keep and revisit.

## Installation

This repository is a [Claude Code plugin marketplace](https://docs.claude.com/en/docs/claude-code/plugins). To install:

1. Add the marketplace:
   ```
   /plugin marketplace add https://github.com/DrCatHicks/learning-goal.git
   ```

2. Install the plugin:
   ```
   /plugin install learning-goal@learning-goal
   ```

3. Restart Claude Code to activate

For more on Claude Code plugins, see the [plugin documentation](https://docs.claude.com/en/docs/claude-code/plugins).

## Why You Might Want to Experiment with This Skill

Most people believe that they know their goals for learning. But in practice, many learning goals fail not because people don't want to achieve them, but because the goals themselves are underspecified, disconnected from real obstacles, and unsupported by concrete plans for what to do when things get hard. This pattern undermines our motivation, and can lead us to struggle when we face friction.

However, the gap between wanting to learn something and actually following through on learning has well-evidenced interventions in empirical psychology. This skill experiments with helping you work through one goal-setting intervention — MCII — inside of your existing workflow. Using this Skill, Claude will walks you through through a short interactive coached exercise that helps you get specific about what you want to learn, visualize why it matters, surface a few of the real obstacles that are most likely to get in your way, and build concrete and actionable if-then plans that help you turn obstacles into action triggers.

## How It Works

Claude offers this exercise when you make an explicit learning goal request ("I want to get better at X," "help me set a learning goal," "how should I approach learning this?") or when you're starting a new project and describing what you want to build. Claude will not offer this mid-task or if you've already declined this session. 

The exercise is conversational and interactive, and intended to force you to do the thinking. This design is aligned with research that shows self-generated goals and obstacles create stronger mental associations than ones suggested to you.

### The Exercise

The exercise moves through these steps, one at a time:

1. **Set a learning goal.** Name a specific skill or area you want to grow in. Claude should help you sharpen vague goals into concrete ones without rewriting them for you.

2. **Strengthen the goal.** Using the SMART framework as a guiding lens, Claude probes the 1-2 dimensions where your goal is weakest. If your goal is already well-formed, this step is brief.

3. **Visualize the outcome.** Briefly describe why this goal matters to you and what changes when you achieve it. Mental contrasting requires pairing a desired future with present reality, and this step establishes the desired future.

4. **Identify obstacles.** You describe real, concrete situations where you'd realistically face obstacles to pursuing your goal. Claude will (hopefully) not suggest obstacles for you. Research shows that specific, real and self-generated obstacles activate stronger cue-response associations, which is the mechanism that makes the intervention work.

5. **Build if-then plans.** For each obstacle, you will draft a specific if-then plan: "If [obstacle/situation], then I will [specific action]." 

6. **Reaffirm or adjust.** After confronting obstacles honestly, does the goal still feel right? Adjusting a goal based on honest reflection is good self-regulation, not failure.

7. **Produce a goal card.** Claude creates a markdown file summarizing your goal, why it matters, your if-then plans, and your first step. This is something you can pin to your project, revisit, or share.

## Pairing with Learning Opportunities

This skill is designed to be independent but pairs naturally with [Learning Opportunities](https://github.com/DrCatHicks/learning-opportunities), a separate Claude Code skill for integrating deliberate practice exercises into agentic coding workflows. 

The two skills serve different functions in the same learning ecosystem. Learning Goal helps you define *what* you're trying to learn and build a motivational plan to persist. Learning Opportunities helps you practice *how* to learn by embedding retrieval, generation, and reflection exercises into your project work. Together, a goal card produced by this skill can inform the learning opportunities Claude offers during your coding sessions, so that Claude already knows what you're working toward.

You can use either skill on its own. They are not dependent on each other.

## The Science Behind It

This exercise is based on Mental Contrasting with Implementation Intentions (MCII), a self-regulation strategy developed by Oettingen and Gollwitzer. The core insight is that positive visualization alone — just imagining success — can actually reduce goal pursuit by satisfying the motivational need without producing action. Mental contrasting corrects this by pairing the desired future with an honest assessment of present obstacles, creating stronger commitment when the goal is feasible.

Implementation intentions — the if-then plans — work by automating the link between a situational cue and a planned response. Instead of relying on in-the-moment willpower, you've already decided what to do when the obstacle appears. The research shows these plans create cue-response associations that operate efficiently even when cognitive resources are depleted. The combination is more effective than either technique alone. 

See PRINCIPLES.md for a full discussion. 

## Customization

This skill can be adapted to your context. You might want to:

- Save your goal card to your project root and reference it in your CLAUDE.md so Claude has your learning goal in context during coding sessions
- Pair it with the Learning Opportunities skill so Claude can connect practice exercises to your stated goals
- Set up a recurring check-in by revisiting your goal card periodically ("read my goal card and help me reflect on progress")
- Adapt it to non-technical learning goals — the psychological mechanism is domain-general and works for writing, design, leadership, communication, or any skill development context

## Background

This skill was developed and adapted by [Cat Hicks](https://www.drcathicks.com/) and [John Flournoy](http://johnflournoy.science/) based on the MCII framework, informed by our work with software teams and across hundreds of people learning technical skills in their real workplaces. 

In [research with thousands of developers](https://osf.io/preprints/psyarxiv/2gej5_v2), we've found that a strong value and commitment to learning predicts that developers feel less threat, worry, and anxiety when imagining needing to adjust to agentic coding. Learning culture also predicts increases in team effectiveness overall, not just individual productivity. Goal setting is a foundational part of that learning culture, and can help individual developers see tangible progress in their learning journeys.

I'd love to know if you find this useful and what you learn! Sharing open science resources helps researchers like me create more things to help software teams. I always appreciate a shout-out or a share, which helps more people learn about the psychology of software teams. Get updates and more at Cat's newsletter: [Fight for the Human](https://www.fightforthehuman.com/)

## Authors

**Dr. Cat Hicks**  
Psychological scientist studying software teams and technology work, author, public speaker, research architect, and empirical interventionist.

- Website: [drcathicks.com](https://drcathicks.com)
- Consulting: [catharsisinsight.com](https://www.catharsisinsight.com/)
- Upcoming Book: *Psychology of Software Teams* (May 2026)

**Dr. John Flournoy**
Research scientist with a focus on statistical methodology, psychometrics, and research computing infrastructure.

Website: [johnflournoy.science](https://johnflournoy.science/)

## Sources

Duckworth, A. L., Grant, H., Loew, B., Oettingen, G., & Gollwitzer, P. M. (2011). Self‐regulation strategies improve self‐discipline in adolescents: Benefits of mental contrasting and implementation intentions. Educational Psychology, 31(1), 17-26.

Gollwitzer, P. M. (1999). Implementation intentions: Strong effects of simple plans. American Psychologist, 54(7), 493.

Gollwitzer, P. M. (2014). Weakness of the will: Is a quick fix possible? Motivation and Emotion, 38(3), 305-322.

Harkin, B., Webb, T. L., Chang, B. P., et al. (2016). Does monitoring goal progress promote goal attainment? A meta-analysis of the experimental evidence. Psychological Bulletin, 142(2), 198-229.

Hicks, C. M., Lee, C. S., & Foster-Marks, K. (2025). The New Developer: AI Skill Threat, Identity Change & Developer Thriving in the Transition to AI-Assisted Software Development. https://doi.org/10.31234/osf.io/2gej5_v2

Inzlicht, M., Werner, K. M., Briskin, J. L., & Roberts, B. W. (2021). Integrating models of self-regulation. Annual Review of Psychology, 72(1), 319-345.

Locke, E. A., & Latham, G. P. (2002). Building a practically useful theory of goal setting and task motivation: A 35-year odyssey. American Psychologist, 57(9), 705-717.

McEwan, D., Harden, S. M., Zumbo, B. D., Sylvester, B. D., Kaulius, M., Ruissen, G. R., ... & Beauchamp, M. R. (2016). The effectiveness of multi-component goal setting interventions for changing physical activity behaviour: a systematic review and meta-analysis. Health psychology review, 10(1), 67-88.

Oettingen, G. (2012). Future thought and behaviour change. European Review of Social Psychology, 23(1), 1-63.

Oettingen, G., & Gollwitzer, P. M. (2010). Strategies of setting and implementing goals: Mental contrasting and implementation intentions.

Pietsch, S., Riddell, H., Semmler, C., Ntoumanis, N., & Gucciardi, D. F. (2024). SMART goals are no more effective for creative performance than do-your-best goals or non-specific, exploratory 'open goals.' Educational Psychology, 44, 946-962.

Toli, A., Webb, T. L., & Hardy, G. E. (2016). Does forming implementation intentions help people with mental health problems to achieve goals? A meta‐analysis of experimental studies with clinical and analogue samples. British Journal of Clinical Psychology, 55(1), 69-90.

Wang, G., Wang, Y., & Gai, X. (2021). A meta-analysis of the effects of mental contrasting with implementation intentions on goal attainment. Frontiers in Psychology, 12, 565202.

## License

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

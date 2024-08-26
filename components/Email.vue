<script setup lang="ts">
import {
  Button,
  Hr,
  Html,
  Text,
  Row,
  Column,
  Section,
} from '@vue-email/components';

defineProps({
  title: String,
});
</script>

<template>
  <Html lang="en">
    <Text>Hello World</Text>
    <Section>
      <Text>Hello World</Text>
    </Section>

    <!-- Formatted with `rows` and `columns` -->
    <Section>
      <Row>
        <Column>Column 1, Row 1</Column>
        <Column>Column 2, Row 1</Column>
      </Row>
      <Row>
        <Column>Column 1, Row 2</Column>
        <Column>Column 2, Row 2</Column>
      </Row>
    </Section>
  </Html>
</template>
